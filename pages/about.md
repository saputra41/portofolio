---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:,<br>
As a Full-Stack Developer with over three years of experience, I have been actively involved in the development of various internal applications within my current company, with a primary focus on backend development using Golang. Before the development phase, I also contribute to system design and feature planning to ensure optimal functionality that meets the product owner's expectations. Additionally, I play a role in DevOps, where I utilize tools such as Podman, Kubernetes (K8s), Jenkins, SonarQube, and Nexus Repository to manage CI/CD pipelines, containerization, and automated deployments. I also have experience in application development using PHP and the Outsystems low-code platform.

In a previous role, I contributed to the development and maintenance of applications for a bank in Indonesia. During this process, I worked closely with clients to understand their business and technical needs, helping to design critical and complex software solutions. I ensure that these solutions are not only functional and aligned with client expectations but also optimized for peak performance in production environments. My approach emphasizes efficiency, scalability, and long-term maintainability.

<style>
  #embed #preview-box.chart-type-table {
    display: inline-block;
    max-width: 100%;
    overflow-x: auto;
  }
</style>

<div class="row">
  <div class="col-12">
    <h2>Programming Skills</h2>
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Golang
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - PHP
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Framework Codeigniter & Laravel
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Outsystems Platform
  </div> 
  <div class="col-md-6 col-sm-12 col-lg-4">
    - PostgreSQL
  </div> 
  <div class="col-md-6 col-sm-12 col-lg-4">
    - MySQL
  </div> 
  <div class="col-md-6 col-sm-12 col-lg-4">
    - jQuery
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - JavaScript
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Kotlin
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - XML
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - JAVA
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Python
  </div>
</div>

<div class="row">
  <div class="col-12">
    <h2>Other Skills</h2>
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Jenkins Pipeline
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Kubernetes
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Docker
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Gitflow
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Github
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Gitlab
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - Bitbucket
  </div>
  <div class="col-md-6 col-sm-12 col-lg-4">
    - REST APIs
  </div> 
</div>

<div class="row" id="embed">
  <div class="col-12">
    <h2>Wakatime Activity (one year)</h2>
  </div>
  <div class="col-12">
    <figure id="preview-box" class="chart-type-table">
      <embed id="embed-wakatime" src="https://wakatime.com/share/@bram41/4ea47abb-b5aa-42ce-8f7a-63b961449097.svg"/>
    </figure>
  </div>
</div>
<div class="row">
{% include about/timeline.html %}
</div>

<script>  
  document.addEventListener('DOMContentLoaded', function() {
    setTimeout(function() {
      var htmlElement = document.querySelector('html');
      var dataTheme = htmlElement.getAttribute('data-theme');
      if(dataTheme == 'dark') {
        document.getElementById("embed-wakatime").setAttribute("src", "https://wakatime.com/share/@bram41/9d706940-8339-4407-a94c-410b68980905.svg");
      } else {                
        document.getElementById("embed-wakatime").setAttribute("src", "https://wakatime.com/share/@bram41/4ea47abb-b5aa-42ce-8f7a-63b961449097.svg");
      }  
    });
  });
  
  const element = document.querySelector('[data-theme]');

  const observer = new MutationObserver((mutations) => {
    mutations.forEach((mutation) => {
      if (mutation.attributeName === 'data-theme' && element.getAttribute('data-theme') === 'light') {
        document.getElementById("embed-wakatime").setAttribute("src", "https://wakatime.com/share/@bram41/4ea47abb-b5aa-42ce-8f7a-63b961449097.svg");
      } else {
        document.getElementById("embed-wakatime").setAttribute("src", "https://wakatime.com/share/@bram41/9d706940-8339-4407-a94c-410b68980905.svg");
      }
    });
  });

  observer.observe(element, { attributes: true });
</script>
