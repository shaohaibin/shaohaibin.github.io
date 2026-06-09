---
layout: page
title: Research
permalink: /projects/
description: 
nav: true
nav_order: 2
display_categories: [AI,Swarm,Network]
horizontal: false
---

<div align="center"><img src="/assets/img/images/logo/logo-SILab.png" style="zoom:18%;"/></div>

<span style="color:black;">欢迎<a href="/publications/">数理基础扎实</a>或<a href="/testbed/">工程能力突出</a>的你申请本科生科研项目、硕士/博士研究生以及<a href="https://postd.sjtu.edu.cn/info/1086/5905.htm">博士后研究员</a>。（如果有任何需要了解请给我发邮件） </span><a href="/opening/"><img src="/assets/img/details_icon.png" style="zoom:15%;"/></a>

<span style="color:red;">2026年、2027年招收具有人工智能、无人系统、航空航天等相关背景的硕士研究生。</span>

I am interested in the **interplay** between the **structure** and **performance** of **complex interconnected systems**, including multidisciplinary scientific and engineering topics such as [**swarm intelligence**](https://en.wikipedia.org/wiki/Swarm_intelligence), [**embodied artificial intelligence**](https://www.techtarget.com/searchenterpriseai/definition/embodied-AI), [**multi-agent systems**](https://en.wikipedia.org/wiki/Multi-agent_system), [**swarm robotics**](https://en.wikipedia.org/wiki/Swarm_robotics), and [**complex networks**](https://en.wikipedia.org/wiki/Complex_network). 

<b> The emergence of collective behavior or even intelligence from individual interactions is a fundamental question across multiple scientific disciplines. </b>
<br/>
<div>
    <div> 
        <a href="https://www.science.org/content/resource/125-questions-exploration-and-discovery" ><img src= "/assets/img/125-science-questions/2021/sjtu-125.png" alt="" width="60" align="left" hspace="10" vspace="0"> </a>
    </div> 
    <span style="color:black;font-size:20px;">What Are Fundamental Principles Of Collective Motion? </span> <br/>
 <span style="color:black;font-size:20px;">How Does Group Intelligence Emerge?</span><br/>
    <a href="https://www.science.org/content/resource/125-questions-exploration-and-discovery" >125 questions: Exploration and discovery. Booklet, Science, 2021.</a> <a href="/assets/img/125-science-questions/2021/sjtu-125.pdf" >[Pages 24,39 PDF]</a>
<div>

</div>
<br/>
    <div> 
        <a href="/assets/img/125-science-questions/2005/science_125.pdf" ><img src= "/assets/img/125-science-questions/2005/science_125.gif" alt="" width="60" align="left" hspace="10" vspace="0"></a>
    </div> 
    <span style="color:black;font-size:20px;"> How Did Cooperative Behavior Evolve?</span><br/>  
       <a href="https://www.science.org/doi/10.1126/science.309.5731.93" >Scientists Researching What We Don't Know.  Vol 309, Science, 2005.</a>  <a href="/assets/img/125-science-questions/2005/science_125.pdf" >[Page 93 PDF]</a>
</div>
<br/>

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
