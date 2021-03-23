To do 

! - details on individual skill or trophy pickup


- Implement resistance to give more challenge than just 1 - 2 - 3 (waiting for cooldowns to go)
- can pickup health to replenish?
- shouts from me (action cries, like "Behaviorism is for pussies" or "I like puzzle games" or "Cross multiplayer game my ass")


? - introduce heated hits; chargeups and release to give extra power.

- change so picking up duplicate skill loot will just give more points to this skill. So you can have 3 points in GD1 for example


x - Push information out when hitting enemy
x Hookup sheet with battle


---------------------
How to Battle CV
**


Enemies are spawned in order from the enemy array. Each x is a new enemy and its properties in y. When enemy is spawned, pop item from array.
If I want randomness in the generation, I can always mix in some in the beginning of the game. 

HUD elements must be anchored correctly to support multiple landscape res. Therefore they must be pinned to sprite which has the anchor. 

TIMELINE BEHAVIOR
Timeline are secretly divided into X steps, relative to its screen width. X = amount of enemies. There is also some margins left and right. Meaning, if user drags timeline, then when dropping, it will snap to one of its steps. Also when automatically defeating someone, it will tween to next step pos. 

FAST FORWARD
When user drags the timeline button, time stops and it shows the correct world title underneath. When dropping the button, button snaps to timeline step and all enemies present are killed, then enemy array are processed one enemy at a time with a delta of very high. Loot and skills are automatically assigned/taken. Result is that game state is now as if user played it to this point. 

FAST BACKWARD
A bit different. Maybe this shouldn't be allowed? 
All skills, trophies, levels are reset to default/erased. Then Enemy Array are reset to default. Then processes as per FAST FORWARD.



SKILL COOLDOWN
Every skill has a cooldown time, where it cannot be used. Therefore a typical sequence is to switch skills all the time and use the skills which are ready.

PLAYER ATTACK
When using a skill on an enemy by touching it while the skill is selected, it dealts damage to the enemy. Screen shake, hp adjusted, red tint, dam number. Attack damage is equal to skill base * skill level reduced by enemy resistances. So if attacking with PM skill X with base dam 20-30 and if level 3 PM and attacking enemy with 20% PM resistance, then dam is random(20-30)*3*0.8.
During its hp range, enemy will spawn some info bits.


ENEMY ATTACK
Enemy also attacks with a base dam and a cooldown. Maybe player attacks can reset the cooldown? When attacking, enemy sprite tweens down towards screen bottom while moving forward in z depth. 
Player hp is adjusted, bar tinted, portrait tinted, maybe screen overall flash red.

ENEMY DEFEAT
When enemy hp is 0 or below, it explodes and loot boxes falls to the floor using physics. Player can now touch to pick each up. 

PICKING UP LOOT
Loot is skills (which gives a new skill + adds a new skill level to player), trophies (which is voiced as achievements) and picture roll. These are one-time only viewings of the project solution (multiple pictures). 
Picking up loot will show loot box opening screen, where player can touch box to open it, revealing its icon and details. It is then added to either skill bar or trophy bar.

PLAYER DEFEAT
If player hp reaches 0 or below, we die. End screen plays with some sad text. 




---------------- char sheet feedback ----------------

add start page, making this my traditional website 
	Me As A RPG Character		Boring oldschool CV		Me Simulated
add random, fabricated? facts
add "click here finger anim"

** 
ikke procent mend bare point
brug flere termer fra rpg sheets

armor class
hp


level x pm, level y gd

 
ratio 
21:9
24:9
*** 

- portrait picture


- pixel explode effect
- sfx 
- go through icons and adjust contrast directly on sprites

- load screen
- format case texts, ie. use uppercase for example
	- links to projects
	- bosses color text hightlight with bbcode
	
- test on all platforms

- use mobile gyroscope for parallax effect

- bg partcile starry sky?


? - possible rpg chat

- add cord to gamepad campaign icon

? mix in fantastic items, to introducice humorrrr

? add support for openeing a few screenshots

x - element z depth tween for singling out elements
x - add retro cursor style on hover
x - stat icons
x add next button on ach+exp pages
x 140 char summary
x remove male
x - more achievements
x - complete case descriptions
