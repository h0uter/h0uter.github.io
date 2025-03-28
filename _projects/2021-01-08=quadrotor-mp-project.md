---
layout: page
title: "Quadrotor Motion Planning"
description: Expanding upon RRT* with a line-of-sight check.
img: /assets/img/PDM_preview.gif
category: uni

github: https://github.com/h0uter/PDM-project

importance: 2
---

<!-- ![wow](/assets/img/PDM_preview.gif) -->
<div align="center">
    <div class="row">
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.liquid path="/assets/img/PDM_preview.gif" class="img-fluid rounded z-depth-1" zoomable=true %}
        </div>
    </div>
    <div class="caption">
        Here you can see the generated path being chased.
    </div>
</div>

In this report we present a comparison between RRT, RRT* and Informed-RRT* path planners in $$R^3$$ for a general quad-rotor. We compare their runtime performance and optimal path cost in two unique environments. We introduce kinodynamic constraints to prevent collisions and evaluate their impact on runtime performance.

[Check out the project on GitHub!](https://github.com/h0uter/PDM-project)

<!-- In short: we built a simulation from the ground up in Python and then implemented RRT and RRT* path planning algorithms to find a path through an obstacle course. Then we simulated a quadrotor to execute this trajectory with a PID controller and chase mode. -->
