---
layout: page
title: abc4d
description: Advanced bolus calculator for diabetes (ABC4D) based on the Case-based Reasoning (CBR) methodology.
img: assets/resources/backgrounds/thumbnails/background-6.jpeg
importance: 3
category: Imperial College London
---

<b>Role:</b> Development of the ABC4D server and deployment on AWS.

<p align="justify">
    The recent increase in the use of technologies such as continuous glucose 
    monitoring (CGM) and self-management mobile apps has led to a digital transformation 
    in diabetes care. However, despite the increasing adoption of these technologies, 
    fewer than one-third of people with Type 1 diabetes achieve their glycaemic targets. 
    Hence, there is an urgent need to empower people living with diabetes with intelligent 
    software tools that can automatically analyse and systematically provide safe, 
    personalized, and effective therapeutic recommendations.
</p>

<p align="justify">
    Insulin bolus calculators have been developed to aid insulin dose adjustment and are 
    currently incorporated in most of the latest commercially available insulin pumps and 
    some glucose meters. Although effective to some degree, they still fall short in achieving
    glycemic therapeutic targets due to the high variability in diabetes management.
</p>

<p align="justify">
    At the Centre for Bio-inspired Technology, we have developed an Advanced Bolus Calculator 
    for Diabetes (ABC4D) that uses continuous glucose monitoring (CGM), Run-to-Run control, 
    and the artificial intelligence technique of Case-based Reasoning (CBR) to overcome these
    barriers.
</p>

<p align="justify">
    The developed insulin recommendation algorithm has been implemented within a mobile app 
    that communicates in real-time with a continuous glucose sensor and requires the user to 
    manually input meals, and physical exercise information to calculate a recommended insulin 
    dose that is tailored to the individual and the current circumstances. The algorithm also 
    adapts its recommendation based on the outcomes of past recommended insulin doses and user
    behavior.
</p>


<div class="row justify-content-sm-center">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.html path="assets/resources/abc4d/graphical-abstract.png" 
        title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm">
        {% include figure.html path="assets/resources/abc4d/img-1.png" 
        title="example image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/abc4d/yoda-demo-2.png" 
        title="example image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/abc4d/yoda-demo-1.png" 
        title="example image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>

<!--
<a href="https://www.imperial.ac.uk/bio-inspired-technology/research/metabolic/abc4d/" class="btn">
    See Post
</a>
-->


<br>

#### Posts

<ul>
    <li>Featured in the <a href="https://www.imperial.ac.uk/bio-inspired-technology/research/metabolic/abc4d/">CBIT newsletter</a></li>
</ul>

<br>

#### Publications

<div class="publications">
   {% bibliography -f conferences -q @*[key=herrero2016demo]* %}
</div>
