---
layout: page
title: '👷‍♂️ PILCO Reproduction'
description: Data efficient reinforcement learning with gaussian processes.
# categories:
#   - projects
# tags:
#   - Reinforcement Learning
#   - AI gym
#   - Python
#   - Gaussian Processes
img: /assets/2021-03-17-Data-Efficient-Reinforcement-Learning-Project/PILCO-linux.jpg
importance: 2
---
 
 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/2021-03-17-Data-Efficient-Reinforcement-Learning-Project/PILCO-linux.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The pendulum simulation in Mujuco
</div>

Currently working on reproducing the [PILCO algorithm](https://www.doc.ic.ac.uk/~mpd37/publications/pami_final_w_appendix.pdf) for reinforcement learning and doing a robustness analysis.

PILCO used Gausian processes for function approximation. One of the main advantages of PILCO is that is promotes data efficient reinforcement learning. 
This is achieved through balancing exploration and exploitation. What this means is that it is able to regulate between generating more data far from its current model (exploration) and generating more data nearby its current model (exploitation).
This is regulated based on how well the target state is captured in the model.
<!-- When the model does not capture the target area of the state space, exploration is prefered. Conversely when the model does capture the target state, generating more data around the target state is prefered. -->
