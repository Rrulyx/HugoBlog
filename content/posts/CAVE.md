---
title: "CAVE System"
date: 2024-02-20T16:55:10+01:00
draft: false
toc: false
images:
tags: 
  - Lecture
---

Here, we study the [CAVE](https://dl.acm.org/doi/abs/10.1145/129888.129892) System. This is an old paper (1992), hence, this system have a lot of limitaions that is due to the state of the hardware at the time, but would be different today. We will nonetheless try to answer a few questions

1. What is the difference between the CAVE System and Head-Mounted Displays? What are their advantages/disavantadges?
2. Where do you think the CAVE fits into the Reality-Virtuality Continuum of Milgram.
3. Does the position in the Reality-Virtuality Continuum changes when more people are experiencing the CAVE
system at the same time?

# Comparison with HMD

The CAVE System is really different from a HMD: it consists in multiple screens placed around the user to represent the virtual world. It displays a picture based on the position of the user so that it matches the right perspective.

Let's look at the major points that differ from the HMD:

## FoV and Panorama

Because the CAVE System is all around the user, it have a full Field of View and allows the user to look in any direction as fast as he wants, contrary to the HMD that need to recompute the scene at each move and that have a limited FoV.

## Body representation

The HMD uses a virtual body whereas the user can see himself in the CAVE system. This can be either a avantage or a disavantage depending on the use case:
- The body is realisitic and perfectly accurate
- The occlusion cannot be changed, meaning the user will never be able to see something close or pick up an object for instance

## Progressive Refinment 

The HMD basically needs to recompute a new scene at each frame, meaning that it will not be able to create a finer render. But if the user does not move it's head to much on a CAVE System, the image can be refined more and more.

This would be really intresting today, as with a bit of time, we can produce photorealistic results and we can use AI to upscale the other results in the mean time, as done in the blender viewport. This could be a real advantage for 3D artists that want to work in VR.

## Collaboration

Because the CAVE System is less intrusive, a small number of user can collaborate on the same device, whereas they would need to have one HMD each to collaborate.

## Other points

The paper also pinpoints other differences, but I feel they are not up to date anymore, for instance the time needed to track the head position, the bad resolution of screens, etc.

## Conclusion

I think the CAVE System is an intresting alternative to HMD, especially for artists who needs to have something that can produce photorealistics renders and need to have a non intrusiove device for long sessions. 

But it stills lacks the possibility to change the occlusion of the hands, which can be a real turndown for all the interactivity... 

# Milgram Continuum

The CAVE System is more of an Augmented Virtuality, close to only virtual, as the only real element you interact with is your body. 

## With more people

When you do collaboration, it tends more towards reality for two reasons:
- You have another real human being in the virtual world.
- The System alone cannot track multiple users at the same time, meaning other users will not have the same presence 
  - With shuttered glasses, the System can quickly alternate between users. But it still can break illusion to notice the screen blinking.

This makes for a really intresting tool for collaboration as often the main issue with collaborating in VR is that you lose the reality and natural facial expressions of the other users.