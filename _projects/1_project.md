---
layout: page
title: Skill Transformer
description: a monolithic policy to solve Habitat Rearrangement tasks. 
img: assets/img/st_example.gif
importance: 1
category: Reinforcement Learning
---

In this project, we leverage offline RL to train a monolithic, end-to-end policy for solving multi-skill, long-horizon tasks such as Habitat Rearrangement. The task involves high-dimensional observation (vision and sensory) and action (10-DoF) spaces, where existing online algorithms struggle to find a solution.

The rearrange-easy task consists of navigating to a random object, picking it up, navigating to the destination, and placing it down.

Below is an example of a rearrange-easy task solved by our end-to-end method.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/st_example.gif" title="example rearrange-easy task" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

This project is in active development. Results on the full rearrange task are forthcoming.

