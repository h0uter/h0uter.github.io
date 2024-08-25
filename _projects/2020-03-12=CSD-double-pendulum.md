---
layout: page
title: 'Pendulum Control'
description: Various controller designs for double pendulum.
img: /assets/2020-03-12-CSD-double-pendulum/dcsc_double_pendulum.jpg
importance: 4
category: uni
---
<div align="center">
    <div class="row">
        <div class="col-sm mt-3 mt-md-0">
    <iframe width="640" height="360" src="https://www.youtube.com/embed/qcokfeDFilA?controls=1&amp;" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>
    <div class="caption">
        (not our video, but same setup. credits: Taamsie)
    </div>
</div>


A double pendulum is studied, where only the first link can be actuated using a motor. Firstly, the system will be modeled using a white-box approach. After determining the equations of motion and state-space equations, the parameters of the system are estimated using an error-function and least-squares fit on generated data. To stabilize the double pendulum in the unstable equilibrium where both links point upwards, the system is linearized around this point. After linearizing and designing an observer, two controllers are designed to stabilize the system around this point. Since the physical setups are not available due to the Coronavirus, all results were analyzed in Simulink.

