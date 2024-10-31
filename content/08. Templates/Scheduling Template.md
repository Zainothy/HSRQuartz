---
date: <%tp.date.now("YYYY-MM-DD",7)%>T<%tp.date.now("HH:mm")%>
tags:
  - Young-Producers
  - Candid-Classics
  - Academia
cssclasses:
  - center-titles
  - center-images
trello_plugin_note_id: MTxITPr4MMpmsGPDdGwVH
trello_board_card_id: 6716b9ef505555cfdca4b8ef;6716ba717c43e3007d34e3fc
---
<%*
let daysAhead = await tp.system.prompt("Enter the number of days ahead for the date (e.g., 8 for 8 days ahead):", "0"); 
daysAhead = parseInt(daysAhead) || 0;%>
## Initial Info:

>[!tip] ### Contextual Information: 
> The following interview will be recorded and produced entirely by a team of OAE Young Producers, the people who are your hosts for Today will be interviewing you in a non-linear, almost conversational format that consists of, but will not be limited to: 
> - Delving into your background and how you made it to this position  
> - Asking questions related to your postion, e.g. challenges you may have faced, etc. 
> Keep in mind the non-linear format of things,  we will make an effort to ensure that you are in tune with us and are properly caught up with the ‘conversation’
> **Finally**, remember that none of this is live: we can adjust anything as necessary in post production processing. 

## Attendees: 
<%* 
// Initialize an empty array to store selected names
let selectedNames = [];
let moreSelections = true;

// Loop to allow multiple selections from the suggester
while (moreSelections) {
  // Show suggester for hosts' names
  let selection = await tp.system.suggester(["Uma", "Sadie", "Mikey", "Zain", "Jessica", "Taylor"], ["Uma", "Sadie", "Mikey", "Zain", "Jessica", "Taylor"]);
  
  // Add selection to the list if it's not already included and not empty
  if (selection && !selectedNames.includes(selection)) {
    selectedNames.push(selection);
    
    // Prompt to continue or stop adding hosts
    moreSelections = await tp.system.prompt("Add another host? Type 'y' to continue or leave blank to finish") === "y";
  } else {
    // Exit the loop if no selection was made
    moreSelections = false;
  }
}
 %>
<% `- **Hosts**: ${selectedNames.join(", ")}` %>
- **Guest**: <% await tp.system.prompt("Who is the guest for today?") %>
 #### Please Bring: 
[Prerequisites]
#### Important Notes: 
[Anything to Note]
# Daily Agenda:

## <% tp.date.now("dddd Do, of MMMM, YYYY", daysAhead)%>
***
**Tasks:**
<%* 
// Ask how many tasks there are
let taskCount = parseInt(await tp.system.prompt("How many tasks are there?"));

// Initialize an array to hold tasks and their time brackets
let tasks = [];

// Loop through the number of tasks to gather details
for (let i = 0; i < taskCount; i++) {
    let taskName = await tp.system.prompt(`Enter the name of task ${i + 1}:`);
    let timeBracket = await tp.system.prompt(`Enter the time bracket for "${taskName}" (e.g., 4:15-4:30):`);
    tasks.push(`- **${taskName}**: ${timeBracket}`);
}

// Output all tasks joined by new lines
tasks.join("\n")
-%>
<% tasks.join("\n") %>

