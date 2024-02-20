---
title: "VRFails"
date: 2024-02-20T14:31:05+01:00
draft: false
toc: false
images:
tags: 
  - Lecture
---

While using VR, you could have different scenarios that could lead to collisions, let's dive into two of them:

# Colision with static objects

In VR, the virtual world does not have the same collisisons as the real world. This can lead to issues, especially in small spaces, where a position empty in VR but have an object in the real world. 

To solve this issue, I propose two solutions :


## Virtual doubles

One option is to create virtual doubles of every object in the real world.

![Virtual Doubles](/HugoBlog/Posts/VRFails/virtualDouble.jpeg)

Each object in the real world have a virtual double and the user tends to avoid them.

There is several issues, one being that it requires a lot of assets to be created, the other being that it is hard to have an open space, for instance a meadow would be hard to create.

## See through

When you move to close to an object, the object appears in your headset to avoid collision.

This is a good option, but it can break the immersion when you see the real object. Furthermore, if the player is doing a fast movement, he will not have enough time to react.

# Loss of balance

For various purposes, you might want to have a different camera orientation on the virtual world than on the real world. This can lead the inner ear to belost and create motion sickness or loss of balance. Let's see how one could fix this:

## A rolling ball

One could use a ball that replicates the motion from the virtual camera in the real world, like [New Atals](https://newatlas.com/vr/eight360-nova-vr-simulator-ball/) does. 

![Eight360](/HugoBlog/Posts/VRFails/360.png)
*The Eight360 Nova*

But this is really expensive and not everybody can have access to this. 

## Remaining seated

Another option is simply to ask the player to sit down before having a big rotation. This could be done by having a virtual double of the player real chair, or by asking him yo sit on the floor.  