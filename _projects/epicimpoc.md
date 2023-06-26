---
layout: page
title: EPiCIMPOC
description: Clinical decision support system (CDSS) to support infection management at the point of care.
img: assets/resources/backgrounds/thumbnails/background-3.jpeg
importance: 1
category: icl

toc:
  - name: Equations
  - name: Citations
  - name: Footnotes
  - name: Code Blocks
  - name: Layouts
  - name: Other Typography?
---

<a href="https://bernardhernandezpe.wixsite.com/epicimpoc/"
   class="" target="_blank">
   Official EPiC IMPOC site
   <i class="fa fa-sm fa-link align-items-right" aria-hidden="true"></i>
</a>

<b>Role:</b> Conceptualization, architect, design, development and deployment on NHS.

<p align="justify">
    EPIC IMPOC is an NIHR i4i funded project which aims to develop intelligent clinical decision support system 
    to help doctors prescribe the most appropriate antibiotics. EPIC IMPOC is a collaborative project between 
    medics and other heathcare professionals from the  National Institute for Health Research Health Protection 
    Research Unit (NIHR HPRU) and engineers from CBIT.
</p>

<p align="justify">
    Healthcare professionals who diagnose and treat infections must often do so rapidly to prevent harm to 
    their patients. Their prescribing decisions can be assisted by providing them with access to treatment 
    recommendations, based on the most likely organism causing the infection (antimicrobial guidelines) and 
    data on local antimicrobial resistance patterns. 
</p>

<p align="justify">
    These decision support systems are mostly rule-based, providing easy-to-access policies or guidelines. A 
    new project started by the Faculty of Engineering and Medicine kickstart scheme, and now funded by the 
    NIHR Invention for Innovation scheme has taken this further, developing anintelligent decision support 
    system. This system is capable of considering a greater number of variables and a more complicated number 
    of scenarios than other systems and by using a machine learning  and artificial intelligence algorithms 
    the system is able to continually learn from its previous experiences.
</p>

<ul>
    <li>The ability to display data from NHS servers on mobile and tablet devices at the patient bedside.</li>
    <li>Algorithms to provide advanced decision support for clinicians for optimised antimicrobial choices.</li>
    <li>A population pharmacometric model to provide individualised antimicrobial dosing.</li>
    <li>Patient engagement tools to facilitate shared decision making across complex health-care pathways</li>
</ul>

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/resources/epicimpoc/cdss-summary.png" 
        title="example image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>

<p align="justify">
    The modular design breaks down the system to reduce its complexity by encapsulating functionality and 
    processes within reusable modules. An overview of these modules, ranging from patient administration 
    and data collection to prognostic functionality is presented below.
</p>

##### Management

<p align="justify">
    The "management" module serves as a central hub or interface that integrates information and data 
    from various submodules such as microbiology, pathology, case-based reasoning, and more. Its primary 
    functionality is to collect, organize, and present this data in a user-friendly manner. Some
    of the key functionality of these modules are: (i) gathers information from different submodules,
    (ii) organizes the information systematically based on different criteria, such as patient cases, 
    medical conditions, or specific areas of interest (iii) provides a user-friendly interface to display 
    the aggregated data, (iv) allows users to add their own notes and annotations to the collected data,
    (v) includes search functionality that enables users to quickly locate specific patients or filter 
    data based on specific parameters and (vi) integration with other software systems or databases, 
    facilitating seamless data exchange and interoperability.
</p>

<div class="row justify-content-sm-center">
    <div class="col-md">
        {% include figure.html path="assets/resources/epicimpoc/cdss-main.png" 
        title="patient table" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/epicimpoc/cdss-therapy.png" 
        title="dose planning" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/epicimpoc/cdss-laboratory.png" 
        title="laboratory results" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm pl-md-1 pl-lg-1 pl-xl-1">
        {% include figure.html path="assets/resources/epicimpoc/cdss-cbr-3.png" 
        title="similar past patients" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>


##### Microbiology

<p align="justify">
    Antimicrobial drugs are commonly used. We have all heard of antibiotics, which fight bacteria, but 
    there are also antifungals, antivirals and antiparasitics that fight fungi, viruses and parasites, 
    respectively. The more we use these drugs, the less effective they become and this problem is known 
    as antimicrobial resistance (AMR). Resistant infections can be difficult, and sometimes impossible, 
    to treat. Antimicrobial susceptibility testing (AST) is a laboratory method used to determine the 
    effectiveness of antimicrobial agents against specific microorganisms. It helps in guiding appropriate 
    antimicrobial therapy by providing valuable information about the susceptibility or resistance of 
    bacteria, fungi, or other pathogens to different drugs. Therefore, the objective of the "microbiology" 
    module has two main aspects. Firstly, it performs automated calculations based on AST data to measure 
    resistance levels, monitor resistance changes over time, assess the effectiveness of different 
    antimicrobials, and more. Secondly, it integrates these metrics into a clinical decision support system, 
    so that healthcare providers can access real-time, data-driven insights to optimize antimicrobial 
    therapy, improve patient outcomes, and mitigate the further development and dissemination of 
    antimicrobial resistance.
</p>

##### Pathology

<p align="justify">
    The "pathology" module is designed to streamline the collection, storage, and visualization of pathology 
    laboratory tests, with a particular focus on scenarios where these tests are conducted frequently, such 
    as on a daily basis. It provides a specialized framework to manage and analyze pathology data in a time 
    series format.
</p>

##### Case-Based Reasoning

<p align="justify">
    In clinical environments, physician reasoning is based on knowledge acquired from past cases 
    personally experienced which is exactly what CBR does! The aim of CBR is to solve new problems 
    based on the solutions of similar past problems in form of cases. CBR is considered a methodology 
    to follow rather than an algorithm in itself. Initially, the CBR methodology requires a set of cases 
    or training examples denoted as case-base. Then, for a specific query, the CBR retrieves those
    cases which are more similar including the treatments and the outcome. 
</p>

##### Probabilistic Inference

<p align="justify">
    In clinical environments, the acute infection management pathway followed by clinicians has been 
    defined as a step-wise Bayesian model in which each step adds systematically information to optimise 
    diagnosis and management of infection. First, they evaluate the physiological parameters of the patient 
    and try to localise and confirm the infection. Then, physicians review and plan further investigations 
    such as pathology laboratory tests, specimen collection for susceptibility testing or imaging. These 
    previous steps allow physicians to construct a clinical picture of the severity of the infection. From 
    this clinical picture, a decision to whether or not to initiate antimicrobial therapy is made with local 
    microbiology guidance as a determinant factor. Finally, an internal and/or external review of the patient
    is conducted to refine the antimicrobial therapy and the entire process is repeated. Thus, the aim of
    this module is to provide support at the different stages of the infection management pathway to assess 
    the likelihoods of a patient having an infection, the location of the infection, the overall 
    severity of the patient and the risk of suffering complications in following days, among others.
</p>

<div class="row">
    <div class="col-6">
        <iframe 
            class="rounded"
            src="https://www.youtube.com/embed/32pTOcXszyg" 
            title="YouTube video player" frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; 
                   picture-in-picture" allowfullscreen>
        </iframe>    
    </div>
    <div class="col-6">
        <iframe 
            class="rounded"
            src="https://www.youtube.com/embed/U-Qb8E4NLuQ" 
            title="YouTube video player" frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; 
            picture-in-picture" allowfullscreen>
        </iframe>
    </div>
    <div class="col-6">
        <iframe 
            class="rounded"
            src="https://www.youtube.com/embed/r4a4ZbbdlDA" 
            title="YouTube video player" frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
            allowfullscreen>
        </iframe>
    </div>
</div>

<br><br>

<br>

#### Posts


<ul>
    <li>Featured in <a href="https://pharmaceutical-journal.com/article/feature/prepare-to-say-hi-to-your-virtual-ai-assistant">The Pharmaceutical Journal</a></li>
    <li>Featured innovative start-up at <a href="https://imperialtechforesight.com/20-futures/tf2040/meta-motivations/">TechForesight 2040</a></li>
    <li>Included within <a href="https://www.imperial.ac.uk/enterprise/staff/techcelerate/participants/cohort-three/"> Techcelerate's 3rd cohort</a> entrepreneurial programme</li>
    <li>Featured in an <a href="https://www.imperial.ac.uk/events/101083/enhanced-personalised-and-integrated-care-for-infection-management-at-the-point-of-care/">ICL seminar</a></li>
    <li>Featured in the <a href="https://www.imperial.ac.uk/bio-inspired-technology/research/infection-technology/epic-impoc/">CBIT newsletter</a></li>
    <li>Information of the <a href="https://fundingawards.nihr.ac.uk/award/II-LA-0214-20008">NIHR funding award </a></li>
    <li>Clinical trial registration in clinicaltrials.gov <a href="https://clinicaltrials.gov/ProvidedDocs/37/NCT04013737/Prot_SAP_000.pdf"> (pdf) </a></li>
    <li>Clinical trial registration in clinicaltrials.gov <a href="https://clinicaltrials.gov/ct2/show/NCT04013737"> (web) </a></li>
    <li>Clinical trial registration in ichgcp.net <a href="https://ichgcp.net/clinical-trials-registry/NCT04013737"> (web) </a></li>
</ul>


<!--
<a href="https://fundingawards.nihr.ac.uk/award/II-LA-0214-20008" class="btn"> NIHR Award  </a>
<a href="https://www.imperial.ac.uk/bio-inspired-technology/research/infection-technology/epic-impoc/" class="btn"> ICL CBIT Post </a>
<a href="https://clinicaltrials.gov/ProvidedDocs/37/NCT04013737/Prot_SAP_000.pdf" class="btn"> Clinical Trial (pdf) </a>
<a href="https://ichgcp.net/clinical-trials-registry/NCT04013737" class="btn btn-outline-primary"> Clinical trial (web) </a>

EPSRC pump priming award, as part of Imperial Antimicrobial Resistance Collaborative (ARC) EMBRACE project,

-->
    
<br>
    
#### Publications
    
<div class="publications">
   {% bibliography -f papers -q @*[key=rawson2021real]* %}
   {% bibliography -f conferences -q @*[key=rawson2019supervised]* %}
   {% bibliography -f theses -q @*[key=hernandez2018data]* %}
   {% bibliography -f papers -q @*[key=hernandez2017supervised]* %}
   {% bibliography -f papers -q @*[key=hernandez2017data]* %}
</div>
