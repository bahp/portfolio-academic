---
layout: page
title: D-CAT
description: Clinical application tool to support dengue management in low and middle income countries.
img: assets/resources/backgrounds/thumbnails/background-1.jpeg
importance: 3
category: Imperial College London
---

<b>Role:</b> Postdoctoral researcher bridging the gap between clinicians and software developers

<p align="justify">
    Dengue epidemics can rapidly increase demand in healthcare services across many endemic settings.
    However, there remains a lack of tools which can rapidly inform patient management and can be
    used at the point of care. Digital clinical decision-support systems (CDSS) allow for efficient
    organisation of care as well as improve the quality of patient management. It is important that these
    tools are designed for the end-user and with the healthcare setting in mind to increase adoption and
    usability.
</p>

<p align="justify">
    We adopted a ground-up human-centred design approach to design a digital CDSS system for
    dengue management in Vietnam (D-CAT). A multidisciplinary team of data scientists, clinicians and
    social scientists were involved in a series of activities designed to map clinical processes, essential
    tasks and decision-making priorities which were crucial in the management of dengue at our hospital
    setting [1]. The desired features for the CDSS identified were: i) patient organisation, ii) availability 
    of guidelines and calculators with easy access, iii) display of results and iv) inference models for dengue 
    diagnosis on admission [2] and further risk-stratification for hospitalised patients based on possible 
    complications [3]. A web-based reactive framework suitable for display on computers and tablets was produced. 
    Priority was placed on usability and modularity so that the system can be re-purposed.
</p>

<p align="justify">
    Dengue Clinical Application Tool (D-CAT) is a bespoke and rapidly scalable CDSS produced following
    clinical pathways, clinician’s needs, and usability in mind. Further work will focus on prospective
    evaluation and iterative improvement of the CDSS including (i) end-user testing and (ii) prospective
    model performance. If successful, the CDSS will be implemented and deployed to evaluate its clinical
    utility.
</p>

<div class="row justify-content-sm-center">
    <div class="col-sm">
        {% include figure.html path="assets/resources/dcat/dcat-01.PNG" 
        title="patient table" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/dcat/dcat-02.PNG" 
        title="dose planning" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/dcat/dcat-03.PNG" 
        title="laboratory results" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm">
        {% include figure.html path="assets/resources/dcat/dcat-04.PNG" 
        title="similar past patients" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/dcat/dcat-05.PNG" 
        title="dose planning" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/dcat/dcat-06.PNG" 
        title="laboratory results" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>


<br>

#### Publications

<div class="publications">
   {% bibliography -f papers -q @*[key=nguyen2023mapping]* %}
   {% bibliography -f conferences -q @*[key=hernandez2022human]* %}
   {% bibliography -f papers -q @*[key=ming2022diagnosis]* %}
   {% bibliography -f papers -q @*[key=ming2022applied]* %}
</div>

