---
Topic: Speed and Breakpoints
tags:
  - HSR
  - "#SpeedAV"
  - SpeedAV
aliases:
  - Speed
  - Breakpoint
  - AV
  - AV Advance
  - Action Value
cssclasses:
  - center-titles
  - no-embed-border
  - image-borders
  - center-images
  - wide-page
share: "true"
---
## Thresholds: 

Thresholds are specific levels of speed stats needed on a character in order to gain a certain amount of actions per cycle, for example. If we wanted 3 turns on a character in cycle 0, we would need 200 speed. 
**Thresholds shown below**
![[../Media/Pasted image 20240816184541.png|Pasted image 20240816184541.png]]

![[../Media/Pasted image 20240816184217.png|Pasted image 20240816184217.png]]

*Credit: Guoba Certified and MrPokke*

Speed can be equated to distance divided by MoC Action Value, this is shown in the above charts. If you wanted to go twice on the first cycle, you would do: 
$${20,000\over150}=133.4$$
	We would do this because, to gain a singular action. A unit needs to move across 10,000 distance: therefore, if we want our unit to move twice we need 20,000 distance to be travelled. We want this distance to be travelled twice in the first cycle, and this means that we would need the unit to travel 20,000 distance within 150 Action Value, because the first cycle of MoC is 150 Action Value. After each cycle, we add 100 AV: 250, 350, 450, etc.

To put this simply, when X= No. of Turns Wanted in Cycle 
$${X {\space}\times\frac{10,000-\text{AV \ Advance}}{AV}}={\text SPD}$$
When given a simple problem like: ‘How much speed is needed for 14 turns across 6 cycles’. We would plug those values into the formula, 6 cycles totals to 650 AV. So we would do $14\times\frac{10,000}{650}=215.384615385$ 

## Action Value Advance: 

Action advance can be thought of as advancing a unit forward in distance, reducing the 10,000 distance units needing to be travelled to gain one action. An example of this being Vonwaq, a 40% advance now requires the unit to travel 6,000 distance. This advance will only occur once. Keeping action advance in mind, we can now apply this to the calculations, if you were using Vonwaq on a unit and want them to take two turns in a cycle. You would subtract 4,000 from the total distance. So instead of it being X * 1000/AV. It would now be:
$$X\times\frac{10000-4000}{AV}$$
**AV Advance cannot go into negatives, an AV Advance of 24,000 at 2000 AV will keep the action gauge stuck at zero, not going into the negatives, not carrying over to the next turn** 
## Speed Buffs: 

Speeds buffs fall under two categories, permanent and temporary. A permanent buff is something that can be kept at 100% uptime, an example being RM’s SPD buff or E1 Huohuo’s Speed buff. Speed buffs are usually additive: meaning that a 10% speed buff from RM, is scaled off of your base speed and not your current speed. If you have 200 speed on a character with 100 base speed, a 10% buff does not mean 20 more speed, it means 10 more. 

Speed buffs allow for speed thresholds to be met more easily. If we need 200 speed to gain 3 actions in a singular cycle, and our base speed is 100 we now need 190 speed as opposed to 200, as RM has increased our speed by 10% of our base speed. 

Temporary speed buffs are more complex, of course. Let’s use TY as an example, who provides a 20% speed buff after her skill is used. Action value is adjusted based on post-buff speed, meaning that the first action that TY takes is unrecoverable AV. TY has already acted, and the speed buff doesn’t equate to starting the cycle with the speed buff, and only affects her for the remaining duration of the buff. 

Here is an example formula for how we can calculate SPD requirements with Temp speed buffs, however this is not always the case as SPD buffs can happen between Action Gauges. It is the most versatile formula available, as there is no one formula that can work for calculating with temporary buffs.

![[../Media/Pasted image 20240817025722.png| Source: Pokke’s Village]]

For TY’s Case, in an EAA Rotation. AV can be calculated like this: 
$$AV={10,000\times(1-\text{TotalAF})\over(SPD+\text Buff \times BaseSPD +FlatBuff )}$$

## Combining and Applying Knowledge: 

Lets say we have TY on 4pc Eagle, S5 DDD, Running an EAA rotation. TY is able to proc eagle and DDD once. I want to calculate the required SPD for ty to go three turns in the first cycle with this setup, in order to do this. We will combine our knowledge to produce this formula. For this formula, another instance of this repeating expression would be added for every single turn that we would want. For example, if we wanted four turns: the number of instances of the expression would be four. 


$$\frac{10{,}000 - AF^1 + AD^1}{SPD + (BaseSPD \times Mod^{1}) + FlatMod^{1}} + \frac{10{,}000 - AF^2 + AD^2}{SPD + (BaseSPD \times Mod^{2}) + FlatMod^{2}} + \frac{10{,}000 - AF^3 + AD^3}{SPD + (BaseSPD \times Mod^{3}) + FlatMod^{3}}=AV
$$

Here is our general formula, after shortening and substituting the equation. We get this, where X=SPD:
$$f\left(x\right)=\frac{10000-4900}{x}+\frac{10000}{x+22.4}+\frac{10000}{x}-150$$
This can then be put into a [graphing calculator](https://www.desmos.com/calculator), and we can find the intercept, this intercept is the breakpoint for 3 turns in cycle zero with the above setup. ![[../Media/Pasted image 20240821000559.png|Pasted image 20240821000559.png]]
	