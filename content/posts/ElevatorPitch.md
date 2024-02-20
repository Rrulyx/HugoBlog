---
title: "Elevator Pitch"
date: 2024-01-14T12:13:27+01:00
draft: false
toc: false
images:
tags: 
  - Pitch
  - SuperMarket
  - Lab
---

# Doctor Octopus

![Octopus](/HugoBlog/Posts/3Techniques/Octopus.png)

I decided to immplement the method where have extendable arm. There is two differents parts to implement: one being the movement, the other being the selection. 
Let's see how I intent on implementing, both of them.

## Selection

The idea behid the selection is that you have a virtual double of your arm that is longer than your original arm, but but points in the same direction.

![Extend arms](/HugoBlog/Posts/ElevatorPitch/extendArm.jpeg)


To implement this, I will look at the vector from the head to the controller and multiply it by some amount to have the position of the virtual hand. Then to select objects, you will be able to just grab them with a button on the controler. 

## Movement

To move, you just push your arm toward the ground and it will anchor in place, letting you orbit around the position of the virtual hand.

![Movement](/HugoBlog/Posts/ElevatorPitch/movement.jpeg)

To implement this, I will check if the virtual hand is underground. 
If so, I will snap it back to the ground and move the player by the same amount I had to move the hand. 
Once the hand anchored, every frame, I will move the player and the virtual hand by the same amount in order to have the virtual hand placed at the anchor point. 
When the player goes down again and move past a certain threshold, I will free the anchor to let the virtual hand move as normal.

## Both at the same time

I think the selection technique will reveal its true potential once the player is confident enough to select and lmove at the same time, one with each handmaking it both precise and fast.

![Both](/HugoBlog/Posts/ElevatorPitch/both.jpeg)
