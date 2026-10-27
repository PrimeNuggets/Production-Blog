---
title: "Lizard Wizard devlog: enemies chase you and it's scary"
author: Georgi
date: 2026-10-27
---
Up to this point the spider and scorpion could spot you, but then they stood there staring at you menacingly. Now they actually chase.

The first attempt was way too strong: full speed instantly, faster than the lizard. So I added a short reaction pause, a speed ramp-up, and turned their speed down a bit. Since you're usually surfing fast, they also aim a little ahead of you to cut you off instead of trailing behind.

They used to give up the moment you went over a dune, so now they see further while chasing and only give up if you get far away or stay hidden for a few seconds.

<iframe
  width="100%"
  height="480"
  src="https://www.youtube.com/embed/9360VooFemw"
  title="Lizard Wizard enemy chase"
  frameborder="0"
  allowfullscreen>
</iframe>