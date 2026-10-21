---
title: Heart/Health UI System and other issues
author: Ibrahim
date: 2026-10-20
---
Fixed an issue that would causes UI elements to not display on the screen properly because of screen size differences. To fix, I set the Canvas Scaler's UI Scale Mode to Scale with Screen Size and Screen Match Mode to Expand.

Additionally, some elements were not set to the UI layer and/or their anchor position needed adjustments.

Added a heart display when coming in contact with enemies, using a specific enemy tag for collider detection. The Script checks to see if the player has any amount of water on them, which then will block any damage they would have taken; this would also have to drain their water in future updates. If they do not have any water, the shield icon is replaced with an unprotected red heart, and the next attack will be fatal. Upon taking a fatal hit, the icon is replaced with a black heart, and the player would faint in the updated version.

<iframe width="1521" height="561" src="https://www.youtube.com/embed/A9Xnr36HPy4" title="2026 10 20 22 33 49" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Issues with the scripts arise when initializing terrain data. Icons don't display properly, and water is cut in half. Opting to merge the health code into the water script and omitting the terrain data from the script at this time. Eventually, will have to make sure when first taking damage after water is drained, the faint icon also doesn't appear.
