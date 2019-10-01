# sc2coop-repo
StarCraft 2 CO-OP suggestions and bug fixes repository.
All trademarks referenced herein are the properties of their respective owners.

Test map with all this and some other changes:
US: `battlenet:://starcraft/map/1/312650`
EU: `battlenet:://starcraft/map/2/219836`

Also I uploaded some CO-OP missions with these changes applied to Arcade. Search “Suggestions Test”.
Some changes require player to enter a command to activate. Full commands list is available via Help menu.

# Chrono bug
A bug where playing as Karax or any other protoss with Karax ally, your second Nexus is not casting chrono boost on itself upon completion. I've made a three variants of how to fix this bug.

#### chrono_bug_normal.SC2Mod
Just a normal fix.

#### chrono_bug_karax_buff.SC2Mod
This variant allows Karax's Crono Wave ability to affect buildings that is under construction.

#### chrono_bug_protoss_buff.SC2Mod
This variant allows Karax's Crono Wave ability and Nexus' Crono Boost ability to be used on buildings that is under construction. The Nexus won't chrono boost itself while constructing.

# Karax
* "-shipswap" command will swap Build Carrier with Artanis' Build Tempest. Fleet Beacon upgrades are swapped too.
#### karax_ex_mod.SC2Mod
* Energizer
  * Added ability to summon Phase Cannon (similar to Karax hero from campaign). Cost 100 energy, cannon exists 30 seconds, cool down 20 seconds.
  * Fixed a minor bug with subgroup priority of Phasing Mode Energizer.
* Level 1 talent
  * Removed gas cost on army upgrades: attack, armor and sields upgrades in Forge and Cybernetics Core.
* Level 11 talent (Instant Pylon/Cannons/Batteries warp)
  * Add 5 range to probe build ability. This will strengthen cannon push strategy for Karax early game.
* Unit Cost Rediction mastery swap with Struscture Cost Reduction (-1% .. -30%)
  * To try this, enter "-mswap" command.

# Alarak
#### alarak_ex_mod.SC2Mod
I tried to implement a mechanics similar to Abathur and Dehaka (the more enemy units is killed, the more powerful they become). Alarak hero unit have enough damage and good offensive abilities, so I though about increasing his defenses.
* Added "Enslaved Souls Armor" to Alarak. This armor becomes stronger when Alarak uses "Soul Absorption" on enemy units.
  * Requires commander level 14.
  * Needs to be researched at Forge: 150/150/90sec. Research require Death Council (Twilight Council).
  * Increases Shield Armor.
  * Increases chance to reflect damage back to the attacking unit (initial chance is 5%). Damage is nullified.
  * Increases damage dealt to attacking unit, when reflection triggered (initial damage is 5).

# Swann
#### swann_ex_mod.SC2Mod
* Pulse Amplifier will now also give Wraith an ability to attack while moving (when "Move" command is used). Unlike Phoenixes, Wraith can't turn while moving.
* Added "Calldown: Extra Supplies" ability to Command Center. Made it cost 100 minerals instead of energy and have 30 seconds cool down. To activate this ability, enter "-supply" command.

# Raynor
#### raynor_ex_mod.SC2Mod
* Added upgrade to Engineering Bay, that allows flying Orbital Command to use Scan.

# Artanis
* "-shipswap" command will swap Build Tempest with Karax's Build Carrier. Fleet Beacon upgrades are swapped too.
* “Superior Warp Gates” passive icon changed into submenu button, that shows all warp in buttons for selected buildings (Gate, Robo, Stargate).

# Zeratul
### zeratul_ex_mod.SC2Mod
* If cannon projection is killed, 120 seconds is added to projection cooldown.
* Telbrus Legion
  * Feedback energy cost is removed and cooldown is 5 seconds. Additionally Telbrus restores shields and energy per damage dealt by Feedback.
  * Some changes to Psi Storm autocast validators (require at least 2 targets)
  * New passive ability "Recall on Death", cost 25 energy from Telbrus, requires comander level 8 and first artifact. When Zealot takes fatal damage, it will be recalled back to Telbrus and restore shileds.
    * when second artifact is found, "Recall on Death" will reset cooldown on Whirlwind and Charge abilities.
    * when third artifact is found, "Recall on Death" will also restore HP of Zealot.
    * it will not work if Telbrus has not enough energy or killed.
* Legon's heroes now have "heroic" tag
* Stasis Beam
  * it will now cast stasis with different duration depending on unit vitals (HP + Shileds)
    * heroic units and units with vitals >= 500: 5 seconds
    * 500 > vitals >= 100: 10 seconds
    * vitals < 100: 15 seconds
  * after stasis units will be debuffed by "Stasis Aftereffect" for 3 seconds
    * slowed and cannot attack or use energy-based abilities
    * 2nd artifact: + 1 to beam width, + 3 seconds to debuff duration, + cloaking is disabled
    * 3rd artifact: + 1 to beam width, + another 3 seconds, + detection is disabled
* Avatar of Form: couldn't think of any other good changes
  * Changed Storm autocast validators (require at lest 2 targets)
  * Storm cooldown reduced to 4 seconds
* Avatar of Essense: a minor change to Devolve autocast filters
