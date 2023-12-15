---
layout: page
title: Teaching
permalink: /teaching/
---

<section class="section projects-section">

   {% for year in site.data.teaching %}
        <div class="intro">
            <p class="section-title">{{year[0]}}</p>
        </div><!--//intro-->
        {% for teach in year[1] %}
         <div class="item">  
            {{teach.name}} - {{teach.term}}
         </div> 
        {% endfor %}
    {% endfor %}


   
</section><!--//section-->
