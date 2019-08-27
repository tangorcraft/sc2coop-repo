# sc2coop-repo
StarCraft 2 CO-OP suggestions and bug fixes repository
All trademarks referenced herein are the properties of their respective owners.

# Chrono bug
A bug where playing as Karax or any other protoss with Karax ally, your second Nexus is not casting chrono boost on itself upon completion.
There is a three variants to fix this bug.

#### chrono_bug_normal.SC2Mod
Just a normal fix.

#### chrono_bug_karax_buff.SC2Mod
This variant allows Karax's Crono Wave ability to affect buildings that is under construction.

#### chrono_bug_protoss_buff.SC2Mod
In addition to the above buff, this variant also allows other protoss commanders to use Nexus' Crono Boost ability to be used on buildings that is under construction. The Nexus won't chrono boosts itself while constructing.

# Karax Suggestions
#### karax_ex_mod.SC2Mod
* Energizer
  * Added ability to summon Phase Cannon (similar to Karax hero from campaign). Cost 100 energy, cannon exists 30 seconds, cool down 20 seconds.
  * Fixed a bug with subgroup priority of Phasing Mode Energizer.
* Level 1 talent
  * Removed gas cost on army upgrades: attack, armor and sields upgrades in Forge and Cybernetics Core.
* Level 11 talent (Instant Pylon/Cannons/Batteries warp)
  * Add 5 range to probe build ability. This will strengthen cannon push strategy for Karax early game.
* Unit Cost Rediction mastery swap with Struscture Cost Reduction (-1% .. -30%)
  * To try this, type "swap" message.
  * I think choosing between cheap structures (for cannon push) vs durable structures (for defence) is better, than choosing between normal price for army units vs durable structures.

# Alarak Suggestion
#### alarak_ex_mod.SC2Mod
I tried to implement a mechanic similar to Abathur and Dehaka (the more enemy units is killed, the more powerful they become). Alarak hero unit have enough damage and good offensive abilities, so I though about increasing his defenses.
* Added "Enslaved Souls Armor" to Alarak. This armor becomes stronger when Alarak uses "Soul Absorption".
  * Increases Shield Armor.
  * Increases chance to reflect damage back to the attacking unit (initial chance is 5%). Damage is nullified.
  * Increases damage dealt to attacking unit, when reflection triggered (initial damage is 5).