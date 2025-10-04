LT-MAKER SKILL REPOSITORY

Note from PKLucky, Repository Manager:
This repository aims to recreate skills from the official Fire Emblem games into LT-Maker WITHOUT the use of custom skill/item components. The following skills are not in this repository. Explanations for their lack of implementation are listed below. Ones that are marked with an asterisk (*) are ones that I think that are possible but I need someone smarter than me to figure it out/jank it.

Aether (Path of Radiance/Radiant Dawn): Proc. Skill - Unit attacks twice. First attack has Sol and second attack has Luna.
   No way to specify the first attack having Sol's properties and the second attack having Luna's properties.

Bane (Radiant Dawn/Engage): Proc. Skill - Reduces enemy's HP to 1.
   Cannot reduce the enemy's HP to 1.

* Blessing (Path of Radiance/Radiant Dawn): Restores MAG amount of HP to adjacent allies at the start of each turn.
* Imbue (Radiant Dawn): Restores MAG amount of HP at the start of each turn.
   Cannot specify the amount of HP to recover based on a Stat.

Blossom (Path of Radiance/Radiant Dawn): Halves EXP gain, but gives each stat that failed to increase on a level up a second chance to increase.
   Cannot invoke level up rerolling.

* Boon (Path of Radiance/Radiant Dawn): At the start of each turn, removes negative status effects from adjacent allies.
   Cannot automatically restore negative status effects/skills.

* Counter (Path of Radiance/Radiant Dawn): Proc. Skill - Target takes half the damage that the user took.
   Cannot get damage taken to then inflict on the foe.

* Corrosion (Path of Radiance/Radiant Dawn: Proc. Skill - Target's weapon durability decreases by one more use.
   There might be a way to do this, actually? Set the Armsthrift component to -1 and get the skill onto the opponent?

Disarm (Radiant Dawn): Proc. Skill - Forcibly unequips the foe's weapon.
   Cannot force unequip a weapon.

* Discipline (Path of Radiance): Prevents user's combat skills from triggering.
   May need a self-Nihil type component. The current Nihil component affects the target only.

* Howl (Radiant Dawn): Proc. Skill - Paralyzes a foe that uses an indirect attack.
* Maelstrom (Radiant Dawn): Proc. Skill - Damages a foe that uses an indirect attack.
* Quickclaw (Radiant Dawn): Proc. Skill - Damages a foe that uses an indirect attack.
* Shriek (Radiant Dawn): Proc. Skill - Negates foe's LCK if attacking indirectly.
   Cannot inflict a status or damage on a foe that the unit cannot counterattack.

Parity (Path of Radiance/Radiant Dawn): Negates all support bonuses, terrain bonuses, and combat skills on both user and foe.
   Cannot negate support bonuses or terrain bonuses

Serenity (Path of Radiance/Radiant Dawn): Halves biorhythm effects.
Tempest (Path of Radiance/Radiant Dawn): Doubles biorhythm effects.
   Not implemented due to biorhythm being a niche mechanic.

Supportive (Fates): If paired up with an ally with a support rank of C or higher, lead unit gets Hit +10, damage dealt +2, and damage taken -2. 
   Support ranks would be project dependent and could also lead to a long conditional check.

########

The following skills are only partially implemented:
Mantle (Radiant Dawn) - Does NOT restore LCK amount of HP at the start of each turn.
Sacrifice (Radiant Dawn) - Drains and restores a set amount of HP rather than dynamically draining and restoring based on the target's current HP.