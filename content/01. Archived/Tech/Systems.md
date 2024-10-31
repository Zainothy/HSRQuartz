---
Topic: Systems Design
aliases:
  - Designing Systems
  - Approach to Design
  - I/O
  - Inputs, Processes, Outputs
tags:
  - School
  - Academia
  - Revision
  - DesignTech
share_link: https://share.note.sx/zrt3vwew#ogmEWEIaDoXJ9NTzPym/84epCsFFlTwpvlek5HsZDMk
share_updated: 2024-07-11T22:22:20+01:00
---
# Approach to Designing: 

>[!context] **Systems revolve around inputs, processes and outputs**: 
> - An input device takes a real world signal like light, sound or movement: and then converts it into an electronic signal like current or voltage 
> - Processes are what goes into receiving an input signal and changing in someway that adds functionality or intelligence to it. 
> - Output devices are in charge of taking signals and converting it back into real world results. An example being how a speaker would output sound 

- Examples of real world inputs include light level, temperature and pressure: 
  Electronic signals may be voltage or current 

<mark class="hltr-blue">  Typically, input devices are switches or sensors</mark>

# Switches: 

>[!info] What are they? 
> <mark class="hltr-green">Switches allow current to flow through them when the contacts within them are connected.</mark> Typically, switches are named after how they work: an example being a push-to-make switch which allows current to flow when pushed. 
> 
> Other examples of switches may include: 
> - <mark class="hltr-red">Reed Switch</mark>
> - <mark class="hltr-purple">Toggle switch</mark>
> - <mark class="hltr-pink">Tilt Switch</mark>

|Type of switch|Uses|
|---|---|
|PTM/PTB switch|Console controller buttons, eg fire or jump|
|Reed (magnetic) switch|Window sensors on alarms, eg window opens and switch contacts open|
|Toggle switch|Power switches|
|Rocker switch|Light switches|
|Tilt switch|To detect if something is no longer level|
>[!info]
>The function of a toggle switch and rocker switch can be exactly the same - it is the shape of the case that determines what the switch is called.
### Sensors

Sensors can be used <mark class="hltr-yellow">to detect changes in light level, temperature and pressure.</mark> There are a wide range of applications for sensors and they are an essential in modern systems design. 

# Micro-controllers 


‘Micro-controllers <mark class="hltr-cyan">provide functionality and give intelligence to products and systems.</mark> From mobile phones to washing machines, many everyday products are controlled by these devices.’’


>[!tip] Purpose of Process Devices: 
>Processors receive the signal from the input source.  
>stage of a system and take action by altering it in some manner, for as by adding a delay, calculating the frequency of an event, or making choices.  
> For this, programmable components like microcontrollers are frequently utilized.


>[!info] Key fact
> A microcontroller is an example of a SBC (single board computer) and is manufactured as an integrated circuit (IC). It can be programmed to perform different processing functions.

Micro-controllers are available in various sizes and have varied numbers of pins—8, 14, and 18—for connecting input and output devices. One common type of micro-controller is the peripheral interface controller (PIC).

## Benefits and drawbacks of Micro-controller use  
### Benefits  
  
- A circuit can be made substantially smaller. This is so because physical components are replaced with code.  
- They are re-programmable multiple times. This makes it possible to make adjustments without having to replace entire parts.  
- To provide flexibility, they feature pins for connecting several input and output devices.  
### Negative aspects  
  
- Frequently, their cost exceeds that of conventional integrated circuits.
- For simple systems, they are consequently not necessarily the ideal choice.  
- Hardware and software programming is necessary. It can be costly to purchase this.  
- The system's language needs to be learnt, which raises the price of training.

#