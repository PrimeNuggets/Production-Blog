---
title: "Desert Spider: Vision and Hearing"
author: Georgi
date: 2026-09-28
---
<p>Last week, our team met, divided up the tasks, and started working on Lizard Wizard full force. Concept art is wrapping up soon™ =)</p>

<p>My main focus has been the concept art and the spider predator’s vision. I used a distance check and a field-of-view angle to decide whether the player is in front of the spider, then a raycast to check its line of sight. I also added a red gizmo in Unity to show the vision range while I test it.</p>

<p>I also added hearing. When the player makes a noise, the spider checks whether it happened within its hearing range. The blue gizmo shows that range in Unity. Right now I’m testing it with the noise the player makes when jumping. Thanks to Xavier for making us a player prefab with physics.</p>

<p>I also put together a simple spider blockout for testing. Its vision still needs some tuning, but it’s been useful to see the detection working in the scene. Here’s a short video of the current prototype:</p>

<iframe width="560" height="315"
  src="https://www.youtube.com/embed/OhYspUQ2a_4"
  title="Lizard Wizard desert spider devlog"
  referrerpolicy="strict-origin-when-cross-origin"
  allowfullscreen></iframe>