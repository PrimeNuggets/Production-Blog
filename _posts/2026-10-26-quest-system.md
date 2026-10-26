---
title: Quest System
author: Xavier
date: 2026-10-26
---
<iframe width="1521" height="561" src="https://www.youtube.com/embed/k4HiCm3gNOI" title="Lizard Wizard - Quests Showcase" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Quests have been fully implemented into Lizard Wizard! A lot of work went into not only this, but the dialogue system had to be reworked to support how quests work.

Quests are given to the player by NPCs through dialogue, with the exception of the tutorial quest, which is assigned to the player as soon as they enter the game scene. Progressing a quest varies depending on it's objective, but the 2 current quests are progressed through the player's controls & talking to the existing NPC.

Quests that are progressed outside of dialogue use a tracking system that keeps track of multiple different things, like how many times the player jumped, if they started a quest, how many quests were completed, etc. In the case of the tutorial quest, it checks if the player jumped at least once.