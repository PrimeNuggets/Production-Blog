---
title: Refactoring Enemy AI
author: Georgi
date: 2026-10-14
---
The enemy AI started with the spider. Xavier had already built much of its state and movement system, including how it switches between behaviors like Search and Wander. I used that work as the starting point for the refactor.

In Stage 2, I moved shared AI code into EnemyAI and split vision and hearing into separate sensors. I also changed hearing so louder sounds can be detected from farther away. When the spider hears the player, it can search toward where the sound came from.

In Stage 3, I moved the state behavior into separate classes. This made EnemyAI smaller and gave each state a clearer place in the code. I tested the spider afterward and fixed a bug where its vision would detect the player jumping but miss them walking.

In Stage 4, I added a scorpion to see whether another enemy could use the same setup. It could, without changes to EnemyAI. That was the main goal of the refactor.  
  
The shared AI structure is in place, though chase movement still needs work. 

![](/Production-Blog/assets/images/REFACTOR_LizardWizard_Modular_AI_UM-2_-_Modular_FSM_Refactor.drawio-4.jpg)

