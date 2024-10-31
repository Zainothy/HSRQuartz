---
Topic: Programming Fundamentals
tags:
  - Computer-Science
  - Programming
  - School
  - Revision
  - Academia
aliases:
  - IF
  - ELSE
  - THEN
Links:
  - "[[Switch Statements]]"
  - "[[Programming Loops]]"
---
# IF Statements: 

>[!context] What are they? 
>If statements <mark class="hltr-pink">are statements in a program that allow you to check if a condition is true, and then carry out a defined action if it is. </mark>
>>[!tip] Example: 
>>
>>```python
>>x = input(“Enter Password”)
>>if x== “GO”: 
>>	print(“Access Granted” )
>> else: 
>>	print(“denied”)
>>```
>>

# Nested IF: 

<mark class="hltr-purple"> Nested IF statements are when an IF statement is placed inside another, these IF statements allow for more checking conditions: once the previous condition has been established as true. </mark>

```python
x=input("Enter Passcode")
if x == "GO": 
	if usertype == "Teacher": 
		print("Unrestricted access granted")
	else:
		print("Restricted Access Granted")
else: 
	print("Access Granted")
```

• IF-ELSEIF statements can also be used to check multiple conditions. They are different from
nested IF statements as they only check more conditions if the previous condition is false.

Sometimes IF Statements aren’t enough, [[Switch Statements]] are typically used when checking Variables to see if they hold a certain value.

