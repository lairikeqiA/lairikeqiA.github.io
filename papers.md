---
layout: page
title: Publications
permalink: /publications/
---

<section class="section projects-section">
    {% for year in site.data.papers %}
        <div class="intro">
            <p class="section-title">{{year[0]}}</p>
        </div><!--//intro-->
        {% for paper in year[1] %}
                <div class="item">
                <span class="project-tagline">[{{paper.idx}}] {{ paper.authors }}. "{{ paper.title }}" <em>{{ paper.venue }}</em>, {{paper.status}}</span>
                </div>
        {% endfor %}
    {% endfor %}
   
</section><!--//section-->