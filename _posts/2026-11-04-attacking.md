---
title: Attacking
author: Xavier
date: 2026-11-04
---
<iframe width="1521" height="561" src="https://www.youtube.com/embed/dfmnj4ZVjeA" title="Lizard Wizard - Attacks Showcase" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Attacking is fully implemented for every entity. However it currently only functions on enemies.

The system includes:

- Damage Application
- Water Drainage
- Palette Infliction
- Knockback Application
- I-Frames (currently unused but attacks ignore invulnerable targets)
- Stun Frames (Both attacker & target)
- Recovery Frames
- Animation Support
- More miscellaneous parameters

A few things to note:

- Attacks are chosen by AI at weighted random
- AI can only choose attacks that are in range of their target. Out of range attacks are not considered in the decision.
- Flags can be defined on attacks but remain dysfunctional until functionality is coded for that specific flag
- Health UI appears for the same amount of time as the recovery time is set for.
- Damage is dealt to water before health
- Knockback functions as so relative to the attacker: X = left(-) / right(+), Y = up(+) / down(-), Z = forward(+) / backward(-)
- Palettes play in order of their definition

