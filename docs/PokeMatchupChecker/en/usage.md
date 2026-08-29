---
layout: default
title: Usage
lang: en
---

# Usage

## 1. App Overview

PokeMatchupChecker is an app that presents type matchups between Pokémon in an easy-to-read table.<br><br>

For each pair of Pokémon in the table, the app displays the type and multiplier of the move with the most favorable type matchup among the moves that Pokémon knows.<br>
You can check type matchups for attacks from ally Pokémon to enemy Pokémon as well as attacks from enemy Pokémon to ally Pokémon.<br><br>

Even beginners who have not memorized every type matchup can see at a glance whether a matchup is favorable.<br>
When building a team, you can use the app to check whether your team includes Pokémon that can handle commonly used threats in the current metagame, or to help choose which Pokémon to bring into a battle.

<div class="notice-box" markdown="1">

**Important Notes**

- Held items are not currently supported.
- Some Ability and move effects are not currently supported in damage calculations.
- We strive to calculate damage correctly for supported Abilities and moves, but accuracy is not guaranteed.
  Please use another website or tool when an exact calculation is required.
- This tool is currently intended for Single Battles only.

</div>

## 2. Main Screen

<img src="../images/main-page_ja.svg" alt="Main screen overview" width="430" style="width: 430px; max-width: 100%; height: auto;">

<div class="table-usage" markdown="1">

| No. | Item | Description |
|---|---|---|
| 1 | Menu | Opens the menu. |
| 2 | [Add](#add-pokemon) | Adds a Pokémon to the Ally Side or Enemy Side. |
| 3 | [Display & Order](#display-order) | Shows or hides Pokémon in the matchup table and changes their order. |
| 4 | Ally Pokémon (rows) | Displays ally Pokémon as rows. Tap a Pokémon to open its [Pokémon Details](#pokemon-info). |
| 5 | Enemy Pokémon (columns) | Displays enemy Pokémon as columns. Tap a Pokémon to open its [Pokémon Details](#pokemon-info). |
| 6 | Matchup Result | Displays the matchup result. See [How to Read the Matchup Table](#how-to-read-matrix) for details about each cell. Tap a cell to open the [Damage Calculation](#damage-calculation) screen for that pairing. |

</div>

The table can be scrolled vertically and horizontally. If many Pokémon are registered, swipe to the row or column you want to view.

## 3. How to Read the Matchup Table {#how-to-read-matrix}

<img src="../images/how-to-read-matrix_ja.svg" alt="How to read the matchup table" width="700" style="width: 700px; max-width: 100%; height: auto;">

<div class="table-usage" markdown="1">

| No. | Item | Description |
|---|---|---|
| 1 | Ally Pokémon | A Pokémon on the Ally Side. |
| 2 | Enemy Pokémon | A Pokémon on the Enemy Side. |
| 3 | Ally's Attack | Displays the type and multiplier of the move with the most favorable type matchup against the enemy Pokémon among the moves the ally Pokémon knows. |
| 4 | Enemy's Attack | Displays the type and multiplier of the move with the most favorable type matchup against the ally Pokémon among the moves the enemy Pokémon knows. |
| 5 | Speed Indicator | A triangle appears on the side with the higher base Speed stat. It is not shown when both base Speed stats are equal.<br>(Because an opponent's build cannot be known in an actual battle, stat points and Nature modifiers are not considered.) |

</div>

Tap a cell to view the calculated damage.<br>
Type matchup multipliers are calculated as follows.
- The multiplier is based on type effectiveness and accounts for certain type-related Abilities, such as Levitate and Thick Fat.
- The same-type attack bonus (STAB) is not included in the multiplier. An option to include it may be added in the future.
- Move effects are not applied.

## 4. Adding Pokémon {#add-pokemon}

<img src="../images/add-pokemon_ja.svg" alt="Steps for adding a Pokémon" width="900" style="width: 900px; max-width: 100%; height: auto;">

<div class="table-usage" markdown="1">

| Step | Item | Description |
|---|---|---|
| 1 | Search | Tap the Add button on the main screen, then enter a Pokémon name in the search field. |
| 2 | Select a Pokémon | Tap the Pokémon you want to add in the search results. |
| 3 | Select a Side | Tap “Add to Ally Side” to register it as an ally Pokémon, or “Add to Enemy Side” to register it as an enemy Pokémon. |
| 4 | Added Pokémon | The Pokémon is added to the selected list, and the matchup table is updated. |

</div>

To change a Pokémon's build, edit it from [Pokémon Details](#pokemon-info).

## 5. Pokémon Details {#pokemon-info}

Tap a Pokémon in a row or column header of the matchup table to view its details.

<img src="../images/pokemon-info_ja.svg" alt="Pokémon Details screen" width="800" style="width: 800px; max-width: 100%; height: auto;">

<div class="table-usage" markdown="1">

| No. | Item | Description |
|---|---|---|
| 1 | Basic Info | View available Abilities, base stats, and weaknesses and resistances by type. |
| 2 | Build Info | View the selected Ability, Nature, stat points, and moves. |
| 3 | Edit | Opens [Edit Pokémon Build](#pokemon-build), where you can change the build. |
| 4 | Delete | Deletes this Pokémon. |

</div>

## 6. Edit Pokémon Build {#pokemon-build}

Tap “Edit” on the Pokémon Details screen to change its build.

<img src="../images/pokemon-build_ja.svg" alt="Edit Pokémon Build screen" width="800" style="width: 800px; max-width: 100%; height: auto;">

<div class="table-usage" markdown="1">

| No. | Item | Description |
|---|---|---|
| 1 | Pokémon Name | Changes the name displayed in lists and the matchup table. |
| 2 | Ability / Nature | Sets the Ability and Nature to use. |
| 3 | Actual Stats & Stat Points | Increase or decrease stat points while checking each resulting stat. Tap “0” or “32” to quickly set that value. |
| 4 | Moves | Tap a move to change it. You can also delete or reorder moves using the “Edit” button. |

</div>

Your changes are reflected in the matchup table and damage calculations.

## 7. Damage Calculation {#damage-calculation}

Tap a cell in the matchup table to open the Damage Calculation screen for that pairing.

<img src="../images/calc-damage_ja.svg" alt="Damage Calculation screen" width="430" style="width: 430px; max-width: 100%; height: auto;">

<div class="table-usage" markdown="1">

| No. | Item | Description |
|---|---|---|
| 1 | Attacker | Displays the stats and types of the attacking Pokémon. |
| 2 | Defender | Displays the stats and types of the defending Pokémon. |
| 3 | Calculation Result | Displays the damage based on the current settings and its percentage of the target's maximum HP. |
| 4 | Settings | Sets the attacker's and defender's moves, number of hits, Abilities, stat points, and other values used in the damage calculation. Use the Attacker and Defender tabs to switch between their settings. |
| 5 | Advantage Setting | Sets whether this pairing should be treated as favorable.<br>Make your own overall assessment based on factors such as Speed and stat adjustments.<br>This setting is reflected in [Team Advantage Check](#advantage-check). |

</div>

Tap the swap button in the center to exchange the attacker and defender and recalculate the damage.

## 8. Matchup Table Display & Order {#display-order}

You can show, hide, and reorder ally Pokémon (rows) and enemy Pokémon (columns) in the matchup table.

<img src="../images/order-visible-setting_ja.svg" alt="Display and order settings screen" width="900" style="width: 900px; max-width: 100%; height: auto;">

<div class="table-usage" markdown="1">

| Step | Item | Description |
|---|---|---|
| 1 | Switch List | Use the tabs at the top to select either the Enemy Side or Ally Side list. |
| 2 | Show, Hide & Reorder | Tap a Pokémon to show or hide it.<br>Drag a Pokémon to change its position in the matchup table. Pokémon are arranged from left to right, starting with the top row. |
| 3 | Finish | Return to the previous screen when you have finished making changes. |
| 4 | Apply Changes | Your changes are reflected in the matchup table. |

</div>

## 9. Team Advantage Check {#advantage-check}

Use the matchup table to see which enemy Pokémon your selected team can fight favorably.<br>
Add an opponent's team or commonly used Pokémon to the Enemy Side, then check whether your selected team can collectively cover them.

<img src="../images/check-matrix_ja.svg" alt="Team advantage check" width="800" style="width: 800px; max-width: 100%; height: auto;">

<div class="table-usage" markdown="1">

| Step | Item | Description |
|---|---|---|
| 1 | Advantage Setting | A pairing marked as “Advantage” on the [Damage Calculation](#damage-calculation) screen is shown in green in the matchup table. |
| 2 | Select Ally Pokémon | Select the checkboxes for the Pokémon you want to include on your team. You can select multiple Pokémon. |
| 3 | Check Enemy Pokémon | The column of an enemy Pokémon is shown in green when at least one selected Pokémon has an “Advantage” matchup against it. |

</div>

---

All rights to Pokémon, related names, characters, trademarks, copyrighted works, and other associated materials belong to The Pokémon Company, Nintendo Co., Ltd., Creatures Inc., GAME FREAK inc., and their respective rights holders.
