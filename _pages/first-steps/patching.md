---
title: "Patching"
layout: single
toc : true
permalink: /first-steps/patching/
sidebar:
  nav: "docs"  
---

Now that you've seen [how to load your 3D file](../#launch), it's time to unleash the power of \_runtime!

From a 3D designer point of view there are always a lot of parameters - colors, channels intensities, reflection, refraction, etc - which needs to be customised by code. 
Code is great but it’s hard to understand and maintain for a 3D designers team.

With \_r you can use patch files to customise the scene. Patch are very easy to read/write text files that don't required any programming skills.

Here a quick example of a patch file content:

```javascript
[
  {
      "scene":
      {
          "ambientColor": "#ffffff",
          "clearColor": "#9CC1CE"
      }
  },
  {
      "cameraFree.000":
      {
          "speed": 0.05,
          "fov": 1.1
      }
  }
]
```