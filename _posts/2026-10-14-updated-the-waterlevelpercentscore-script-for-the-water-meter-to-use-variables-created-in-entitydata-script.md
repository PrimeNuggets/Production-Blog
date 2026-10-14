---
title: Updated the WaterLevelPercentScore script for the Water Meter to use
  variables created in EntityData script.
author: Ibrahim
date: 2026-10-14
---
Essentially, everything is the same, just some under-the-hood reassignment to use Stat water from EntityData. There were some issues because of NonSerialized/SerializeField usage and other parameters that I didn't immediately know what to do about it.

In Unity, the EntityData's water stat in parameters was set to 0 and wasn't updated, so my code was just dividing by zero, which is why the meter wasn't draining properly. By setting it to the given maximum, that issue was fixed.

![image.png](/Production-Blog/assets/images/image.png)

