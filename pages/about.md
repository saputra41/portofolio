---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:,<br>
As a Full-Stack Developer with two years of experience, I have been involved in developing and maintaining applications for a major bank in Indonesia. I actively engage with clients, both on the business and technical aspects, to develop critical and complex software solutions that are functional, meet expectations, and perform well in the client's production environment.

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
  <div class="col-md-4">
    - PHP
  </div>
  <div class="col-md-4">
    - Framework Codeigniter
  </div>
  <div class="col-md-4">
    - Framework Laravel
  </div>
  <div class="col-md-4">
    - MySQL
  </div> 
  <div class="col-md-4">
    - jQuery
  </div>
  <div class="col-md-4">
    - JavaScript
  </div>
  <div class="col-md-4">
    - Kotlin
  </div>
  <div class="col-md-4">
    - XML
  </div>
  <div class="col-md-4">
    - JAVA
  </div>
  <div class="col-md-4">
    - Python
  </div>
</div>

<div class="row">
  <div class="col-12">
    <h2>Other Skills</h2>
  </div>
  <div class="col-md-4">
    - Gitflow
  </div>
  <div class="col-md-4">
    - Github
  </div>
  <div class="col-md-4">
    - Gitlab
  </div>
  <div class="col-md-4">
    - Bitbucket
  </div>
  <div class="col-md-4">
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