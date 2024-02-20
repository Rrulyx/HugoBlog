---
title: "Selection Techniques"
date: 2024-02-20T18:24:31+01:00
draft: false
toc: false
images:
tags: 
  - Lecture
---

# Bubble Mechanism

[Link](https://ieeexplore.ieee.org/document/9089485)

This selection technique is a mix between a bubble cursor and a Ray-casting method. The idea is to chose the closest object to the ray going from the controller. (Closest being either euclidian distance or angular distance)

![Bubble](/HugoBlog/Posts/Selection/Bubble.png) 

- **Reach:** infinite (the ray can be as long as needed)
- **Cardinality:** Single
- **Progressive refinement:** Continuous (The bubble changes size continously)

# SQUAD

[Link](https://ieeexplore.ieee.org/abstract/document/5759219)

In this Selection techniuqe, you begin by using a sphere to create a encapsulate loosely your object. The sphere position is determined by a ray casting method. The radius of the sphere being higher the furthest it is from camera.

![Bubble](/HugoBlog/Posts/Selection/SQUAD1.png) 

But because you also might have other objects in the sphere, You need to refine your choice by selecting where is your object among the 4 quarters.

![Bubble](/HugoBlog/Posts/Selection/SQUAD2.png) 

You do this until you only have your object.

- **Reach:** infinite (the ray can be as long as needed)
- **Cardinality:** Single
- **Progressive refinement:** Discrete (Tou divide the number of items by 4 each time)

# iSith

[Link](https://ieeexplore.ieee.org/document/1647507)

In this Selection technique, you have one ray on each hand and you select the object closest to the projected intersection of this rays.

![Bubble](/HugoBlog/Posts/Selection/iSith.png) 

- **Reach:** Technically infinite (the rays can be as long as needed, but the intersection is hard to finetune if far away from the handles)
- **Cardinality:** Single
- **Progressive refinement:** None
