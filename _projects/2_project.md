---
layout: page
title: Robot Motion Planning Algorithms
description: A collection of 4 different motion planning methods for a differential drive on a 2D maze example.
img: assets/img/q5.png
importance: 2
category: Course projects
---
This is a motion planning repo adopted from HW5 of [CSE276C Mathematics in Robotics (FA22)](http://www.hichristensen.net/CSE276C-22/index.html) at UCSD. Following motion planning algorithms are involved:

* Dijkstra's algorithm
* Voronoi diagram path planning
* Probabilistic roadmap (PRM) path planning
* Rapidly exploring random tree (RRT)

GitHub repo [here](https://github.com/Joyyy821/motion-planning-zoo) (Note: the project repo is **NOT permently public**. It could be set to **private** as required by the course instructor. This page demostrates some main results from my project.)

## Shortest Path

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/q2_on_0_90_cspace.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/q2_on_45_cspace.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The shortest path found by Dijkstra's algorithm. The figure on the top shows the shortest path in the configuration space when robot facing east, west, south, or north. The figure on the bottom shows the shortest path in the configuration space when robot facing northeast, northwest, southeast, southwest.
</div>

## Safest Path

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/q3_voronoi.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The safest path found by using Voronoi diagram.
</div>

## Probabilistic Road-Map (PRM)

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/q4_500samples.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The path found by using PRM with 100 samples.
</div>

## Rapidly-Exploring Random Trees (RRT)

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/q5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The path found by using RRT with the step size (extension length to put the new node) equals to 5 and the probability of sampling the goal-point equals to 5%.
</div>
