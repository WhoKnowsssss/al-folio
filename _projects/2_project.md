---
layout: page
title: Multi-agent FPS Game AI
description: a multi-agent game AI with RL in the context of a toy FPS game. 
img: assets/img/fps_cover.gif
importance: 2
category: Reinforcement Learning
---

While working at Tencent, we developed a multi-agent game AI in a 3D First Person Shooting game that imposes distinct roles and strategies on the agents. Here're some demonstrations in a toy environment ( as the actual game was subject to NDA... )

An attacker trys to avoid shoots from a static defender. 
(For easier illustration, we use top-down view. The green agent's egocentric view is in the depth map on the top-right. )

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fps1.gif" title="1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

We utilized PPO with mutual information sharing in a two-agent competition setting. We trained the attacker and defender policies with self-play to
achieve self-supervised learning, without designing a delicate opponent. 

The attacker and defender try to peak at each other and get a tie. 
(The blocks between them are walls)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fps2.gif" title="1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

In the final results, our method achieved human-player level performance on simple settings, measured by Elo score. 

Some interesting switching sides between the attacker and the defender with some walls between them. 
(The blocks between them are walls)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fps3.gif" title="1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

