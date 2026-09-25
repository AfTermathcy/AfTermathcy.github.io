---
layout: homepage
permalink: /
title: "Chengyue He"
body_class: academic-home
redirect_from:
  - /about/
  - /about.html
---
{% include base_path %}
<section id="about" class="home-intro" aria-labelledby="intro-title">
<div class="intro-copy" markdown="1">
<h1 id="intro-title">Chengyue He</h1>

Hi, hope you have a great day!

I am a Postdoctoral Researcher in the Department of [Industrial Engineering & Management Sciences](https://www.mccormick.northwestern.edu/industrial/) at <span class="northwestern-name">Northwestern University</span>, working with Professor [Simge Küçükyavuz](https://users.iems.northwestern.edu/~simge/).

I obtained my Ph.D. in the Department of [Industrial Engineering and Operations Research](https://ieor.columbia.edu/) at <span class="columbia-name">Columbia University</span>, where I was fortunate to be advised by Professor [Yuri Faenza](https://www.columbia.edu/~yf2414/) and Professor [Jay Sethuraman](https://www.columbia.edu/~js1353/).

During my Ph.D., my research focused on **discrete optimization, matching markets and mechanism design**, with applications including stable matchings, school choice, kidney exchange programs, and strategic behaviors.

</div>
<aside class="intro-profile" aria-label="Photo and contact links">
  <div class="portrait-frame"><img class="intro-photo" src="{{ base_path }}/images/{{ site.author.avatar }}" alt="Chengyue He holding a camera at Glacier National Park" fetchpriority="high"></div>
  <p class="photo-caption">@ Glacier National Park, MT</p>
  <p class="profile-email">chengyue [dot] he [at] northwestern [dot] edu</p>
  <div class="profile-links">
    <a href="{{ base_path }}/files/Chengyue_CV_202512.pdf" aria-label="Curriculum vitae">CV</a>
    <a href="{{ site.author.googlescholar }}">Google Scholar</a>
    <a href="https://github.com/{{ site.author.github }}">GitHub</a>
    <a href="https://www.linkedin.com/in/{{ site.author.linkedin }}/">LinkedIn</a>
  </div>
</aside>
<details class="home-news" open>
<summary>Recent News/Upcoming Talks</summary>
<div markdown="1">

- August 2026: I successfully defended my dissertation, "Scarf’s Algorithm and Its Application to Stable Matchings"! 🎉
- October 2025: I host a session "Optimization and Strategic Issue in Matching Markets" at INFORMS Annual Meeting at Atlanta.
- September 2025: Our work ["Minimum Cut Representability of Stable Matching Problems"](https://arxiv.org/abs/2504.04577) has been awarded honorable mention in the INFORMS Optimization Society's 2025 Student Paper Prize!
- July 2025: I give a talk at [ICALP 2025](https://conferences.au.dk/icalp2025) on our paper ["Scarf's Algorithm on Arborescence Hypergraphs"](https://arxiv.org/abs/2412.03397).
- May 2025: Our paper ["Scarf's Algorithm and Stable Marriages"](https://doi.org/10.1287/moor.2023.0055) has been accepted for publication on Mathematics of Operations Research.

</div>
</details>
</section>
<section id="education" class="home-section" aria-labelledby="education-title">
<h2 id="education-title">Education</h2>
<div class="section-content">
  <div class="education-entry"><div><h3><span class="columbia-name">Columbia University</span></h3><p>Ph.D. in Operations Research</p></div><span class="entry-date">2021–2026</span></div>
  <div class="education-entry"><div><h3><span class="columbia-name">Columbia University</span></h3><p>M.S. in Operations Research</p></div><span class="entry-date">2019–2020 😷</span></div>
  <div class="education-entry"><div><h3><span class="zhejiang-name">Zhejiang University</span></h3><p>B.S. in Mathematics</p></div><span class="entry-date">2015–2019</span></div>
</div>
</section>
<section id="publications" class="home-section" aria-labelledby="publications-title">
<h2 id="publications-title">Publications<br> &amp; preprints</h2>
<div class="section-content">
{% assign publication_groups = "Manuscripts,Journal Articles,Conference Proceedings" | split: "," %}
{% for group in publication_groups %}
  {% assign papers = site.publications | where: "publication_group", group | sort: "display_order" %}
  <h3 class="publication-category">{{ group }}</h3>
  {% for post in papers %}
  <article class="publication-entry">
    <p class="publication-venue">{% if post.is_published %}{{ post.venue }} · {{ post.publication_year }}{% else %}{{ post.status }}{% endif %}</p>
    <h4><a href="{{ post.paperurl }}">{{ post.title }}</a></h4>
    <p class="publication-authors">{% for author in post.authors %}{% unless forloop.first %}{% if forloop.last %}{% if post.authors.size > 2 %},{% endif %} and {% else %}, {% endif %}{% endunless %}{% if author == "Chengyue He" %}<span class="author-self">{{ author }}</span>{% else %}{{ author }}{% endif %}{% endfor %}</p>
    <details class="publication-abstract">
      <summary>Abstract</summary>
      <p>{{ post.abstract | escape }}</p>
    </details>
    <a class="paper-link" href="{{ post.preprint_url }}">{{ post.preprint_label }}<span class="sr-only">: {{ post.title }}</span></a>
  </article>
  {% endfor %}
{% endfor %}
</div>
</section>
<section id="teaching" class="home-section" aria-labelledby="teaching-title">
<h2 id="teaching-title">Teaching</h2>
<div class="section-content" markdown="1">

### Instructor
* Graph Theory by Example (Science Honors Program at Columbia Engineering)
  * PhDs and postdocs in the sciences and mathematical disciplines teach courses in their area of study aimed at high school students.
  * Spring 2022, Fall 2021


### Teaching Assistant
* IEOR 3609 Advanced Optimization (Undergrad course)
  * Spring 2025
* IEOR 6613 Optimization I (PhD level course)
  * Fall 2024, Fall 2023

</div>
</section>
<section id="personal" class="home-section" aria-labelledby="personal-title">
<h2 id="personal-title">Personal<br> miscellany</h2>
<div class="section-content personal-content" markdown="1">

### Name

My name is Chengyue He (何呈栎), pronounced “Chuhng-yweh Huh.” Feel free to call me by my Starbucks name, Hector.

### Good hobbies, but by no means good at

Cooking, tennis, hiking, and photography.

### Bad hobbies, but partly good at

I have [three furry kids](https://www.instagram.com/amberbenbendoubao/).

I play [poker](https://pokerdb.thehendonmob.com/player.php?a=r&n=1203343). Before that, I played [Dota 2]({{ base_path }}/images/dota-2-divine-i.png).

</div>
</section>
