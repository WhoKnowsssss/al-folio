---
layout: page
title: Multi-agent FPS Game AI
description: a multi-agent game AI with RL in the context of a toy FPS game. 
img: assets/img/fps_cover.gif
importance: 2
category: Reinforcement Learning
---

While working at Tencent, we developed a multi-agent game AI for a 3D first-person shooting game that assigns distinct roles and strategies to each agent. Below are some demonstrations in a toy environment (the actual game is under NDA).

An attacker tries to dodge shots from a static defender.
(For easier illustration, we use a top-down view. The green agent's egocentric view is shown in the depth map on the top right.)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fps1.gif" title="1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

We utilized PPO with mutual information sharing in a two-agent competitive setting. The attacker and defender policies are trained via self-play, achieving self-supervised learning without requiring a hand-designed opponent.

The attacker and defender try to peek at each other, resulting in a tie.
(The blocks between them are walls.)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fps2.gif" title="1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Our method achieved human-player-level performance on simple settings, as measured by Elo score.

An interesting example of the attacker and defender switching sides with walls between them.
(The blocks between them are walls.)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fps3.gif" title="1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

