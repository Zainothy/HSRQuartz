---
Topic: Electricity
tags:
  - School
  - Academia
  - Physics
  - Revision
aliases:
  - Paralllel
  - Series
Links:
  - "[[Electricity (Section 2)]]"
  - "[[Key Terms]]"
  - "[[Ohm's Law]]"
---
# Series and Parallel Circuits: 


> [!note] What’s the difference? 
> A series circuit is a <mark class="hltr-cyan">single loop</mark> where the <mark class="hltr-pink">components are connected one after the other</mark>. Parallel circuits on the other hand, contain more than one loop: this small difference completely overhauls how we measure current, voltage and resistance. ^Diff

## Series Circuits: 

- <mark class="hltr-blue">All components are in a single loop</mark>, this can be a downside: if one component in the loop malfunctions or is disconnected, the whole circuit will no longer function. 

- The <mark class="hltr-red">potential difference of the battery or cell, is shared across all components</mark>. This means we can calculate the total Pd using this equation $$Vtotal=V_{1}+V_{2}+V_{3}\dots$$
- <mark class="hltr-green">Current, is the same everywhere in the circuit, no matter what. </mark>Current is measured using an ammeter, which is placed in series. The current is the same everywhere, so we can place an ammeter in any part of the circuit. 

- We can also calculate current using a rearranged form of Ohms Law: $I=\frac{V}{R}$

- The formula for calculating resistance in a series circuit is simple, <mark class="hltr-yellow">it is the sum of the individual resistances in each component. </mark>
	- $\sum \text{Of individual resistance in each component}$
	- After calculating resistance, we can use Ohms law to calculate current. 


> [!tip] Calculating Voltage in components…
> After working out the current of a circuit using Ohm’s law, we can use that current: because <mark class="hltr-pink">resistance stays the same across the entire circuit</mark>. Then, we can use the resistance of the individual component and<mark class="hltr-purple"> use $V=IR$ to work out the Voltage </mark> 
> > [!note] Another way: 
> > A final way that one can measure voltage is: using a voltmeter, <mark class="hltr-red">they are connected in parallel to the circuit </mark>

# Parallel Circuits: 

- It is common for parallel circuits to have an entire loop per components, this can also lead to less failures as the loop will continue to function even if a component breaks. 
	- However, circuits will typically have series and parallel properties, so u may have multiple loops but several components in one. 

> [!info] Voltage is a bit.. different: 
>
> The thing about truly parallel circuits (all circuits are in parallel), is that voltage is the same across every component, it is not shared. means that: $$V_{total}=V_{1}=V_{2}=V_{3}\dots$$
>> [!tip] Current!
>> Current is shared between loops, this means that if a circuit with 2 loops had a total current of  $4A$, the the current in one loop there may be three amps, and another has 1. This means the formula for current is: $$I_{Total}=I_{1}+I_{2}+I_{3}\dots$$ 
>> How the current splits is entirely dependent on resistance, currents with a greater resitance will  get a smaller share of the currents 
>
>
>>[!warning] And finally.. resistance 
>Oddly, the more components added in parallel: the lower the total resistance will be. This is because it provides extra paths for the charge to flow. This applies even when the parallel circuits contain resistors.
 