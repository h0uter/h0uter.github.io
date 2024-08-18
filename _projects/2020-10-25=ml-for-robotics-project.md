---
layout: page
title: 'Cutlery Classifier'
description: End-to-end ML pipeline for robot gripper.
img: /assets/img/ml_knife.png
category: uni
importance: 2
---


You can execute our code yourself on [Deepnote](https://deepnote.com/project/452790e4-76c0-49f0-8fb0-80760653c8f0)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/ml_knife.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The lines show the distinct detections of the handle and the blade of the knife.
</div>


A small robot gripper has to detect cutlery and determine a suitable grip pose. To this end a computer vision pipeline was constructed.

The general ML cookbook looks something like this:

1. **Overview**
  - make a plan
2. **get the data**
	- representiveness
	- need to annotate
	- use simulation to obtain data (well suited for reinforcement learning)
	- check possibilities for data augmentation data augmentation
3. **Inspect Data, gain insights**
	- GOAL: develop intuition
	- find outliers
	- determine physical meaning
4. **Prepare data**
	- GOAL: expose the underlying patterns to the ML algorithm
		- how2translate 'task' to 'ML problem'
	- Feature selection/ feature engineering
	- what do the measurements represent
	- data compression
		- which variance is informative
		- which variance can be removed
	- data transforms to deal with:
		- missing values
5. **Explore different models**
	- for robotics fast inference required as part of control loop
	- training time more forgiving
	- "more data vs. better model" ROI consideration
6. **Fine tune your model**
	- Optimise hyperparameters
7. **Present your solution**
	-  ensure results are reproducible
8. **Launch, monitor and maintain your system**

Additionally, we compared the performance of classical ML methods with newer DL methods and our results can be seen in the published notebook.
