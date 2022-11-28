---
layout: page
title: Skill Transformer
description: a monolithic policy to solve Habitat Rearrangement tasks. 
img: assets/img/st_example.gif
importance: 1
category: Reinforcement Learning
---

In this project, we leverage offline RL to train a monolithic, end-to-end policy to solve multi-skill long-horizon tasks, like Habitat
Rearrangement. The task involves high-dimensional observation (vision & sensory) and action (10DoF) spaces, and existing online
algorithms were are to solve it.

The rearrange-easy task consists of navigating to a random object, picking it up, then navigating to the destination and dropping it. 

An example of a rearrange-easy task solved by our end-to-end method. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/st_example.gif" title="example rearrange-easy task" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

 The project is in active development. More results in the full rearrange task are coming up. 

