---
layout: about
title: about
permalink: /
subtitle: B.S. Candidate in Artificial Intelligence · Yonsei University

selected_papers: false
social: false
detail_pages_enabled: true

announcements:
  enabled: false
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

<div class="academic-home">
  <aside class="academic-profile" aria-label="Profile">
    <img class="profile-photo" src="{{ '/assets/img/xingyi-pu-portrait.png' | relative_url }}" alt="Portrait of Xingyi Pu" width="1024" height="1536" fetchpriority="high">
    <p class="profile-eyebrow">YONSEI UNIVERSITY</p>
    <h1 class="profile-name">Xingyi Pu</h1>
    <p class="profile-role">B.S. Candidate<br>Artificial Intelligence</p>
    <p class="profile-affiliation">Yonsei University</p>

    <div class="profile-links">
      <a href="mailto:{{ site.data.socials.email }}">{{ site.data.socials.email }}</a>
      <a href="https://github.com/{{ site.data.socials.github_username }}">GitHub</a>
      <a href="https://www.linkedin.com/in/{{ site.data.socials.linkedin_username }}/" rel="me">LinkedIn</a>
    </div>

    <nav class="profile-index" aria-label="On this page">
      <p>On this page</p>
      <a href="#biography">Biography</a>
      <a href="#research-interests">Research interests</a>
      <a href="#selected-projects">Selected projects</a>
      <a href="#education">Education</a>
      <a href="#honors">Honors &amp; awards</a>
      <a href="#experience">Additional experience</a>
    </nav>

  </aside>

  <div class="academic-content">
    <section id="biography" aria-labelledby="biography-heading">
      <h2 id="biography-heading">Biography</h2>
      <p>
        I am an undergraduate student in <strong>Artificial Intelligence at Yonsei University</strong>, based in Seoul, South Korea. My interests span
        <strong>artificial intelligence, the Internet of Things (IoT), and intelligent systems</strong>. I enjoy exploring new ideas, learning unfamiliar
        technologies, and combining intelligent software with connected devices to solve practical problems.
      </p>
      <p>
        I am currently developing a {% if page.detail_pages_enabled %}<a href="{{ '/projects/00-smart-medication/' | relative_url }}">smart medication management system</a>{% else %}smart medication management system{% endif %}, exploring a
        Bluetooth-enabled pillbox concept and a WeChat Mini Program for reminders and user interaction. I also remain interested in intelligent vehicles
        and sustainable transportation, particularly learning-based perception and decision-making for safer, more efficient mobility.
      </p>
      <p>
        My preparation spans programming, machine learning, mathematics, and computer systems. I am currently strengthening my foundations in sensor
        fusion and intelligent transportation systems.
        {% if page.detail_pages_enabled %}More about my <a href="{{ '/research/' | relative_url }}">research interests and academic foundations</a>.{% endif %}
      </p>
      <p class="academic-invitation">
        I welcome opportunities to develop my research and technical skills in AI, IoT, intelligent mobility, and connected systems.
      </p>
    </section>

    <section id="research-interests" aria-labelledby="research-heading">
      <h2 id="research-heading">Research interests</h2>
      <ul class="research-list">
        <li><strong>AI and connected devices.</strong> Intelligent software, IoT, medication reminders, digital tracking, and smart healthcare applications.</li>
        <li><strong>Autonomous driving.</strong> Deep learning, sensor fusion, obstacle detection, path planning, and real-time decision-making.</li>
        <li><strong>Vehicular communication.</strong> V2V and V2I systems for safer and more coordinated traffic.</li>
        <li><strong>Human-vehicle interaction.</strong> Intuitive interfaces and trustworthy interaction in semi-autonomous and autonomous vehicles.</li>
        <li><strong>Sustainable transportation.</strong> AI-assisted route optimization, emission reduction, electric mobility, and smart-city integration.</li>
      </ul>
    </section>

    <section id="selected-projects" aria-labelledby="projects-heading">
      <h2 id="projects-heading">Selected projects</h2>
      <div class="project-list">
        {% assign selected_projects = site.projects | sort: 'importance' %}
        {% for project in selected_projects limit: 3 %}
          <article class="project-entry">
            <h3>{% if page.detail_pages_enabled %}<a href="{{ project.url | relative_url }}">{{ project.title }}</a>{% else %}{{ project.title }}{% endif %}</h3>
            <p>{{ project.description }}</p>
            <div class="project-links">
              {% if page.detail_pages_enabled %}<a href="{{ project.url | relative_url }}">Overview</a>{% endif %}
              {% if project.github %}
                <a href="{{ project.github }}">Code <span aria-hidden="true">↗</span></a>
              {% endif %}
            </div>
          </article>
        {% endfor %}
      </div>
      {% if page.detail_pages_enabled %}<p class="section-more"><a href="{{ '/projects/' | relative_url }}">All projects <span aria-hidden="true">→</span></a></p>{% endif %}
    </section>

    <section id="education" aria-labelledby="education-heading">
      <h2 id="education-heading">Education</h2>
      <div class="academic-record">
        <div class="record-date">Sep. 2022–Present</div>
        <div class="record-body">
          <h3>Yonsei University</h3>
          <p>B.S. in Artificial Intelligence</p>
          <p>Expected graduation: August 2027</p>
        </div>
      </div>
    </section>

    <section id="honors" aria-labelledby="honors-heading">
      <h2 id="honors-heading">Honors &amp; awards</h2>
      <div class="academic-record">
        <div class="record-date">Autumn 2023</div>
        <div class="record-body"><p>Artificial Intelligence Faculty Support Scholarship</p></div>
      </div>
    </section>

    <section id="experience" aria-labelledby="experience-heading">
      <h2 id="experience-heading">Additional experience</h2>
      <div class="academic-record">
        <div class="record-date">Early 2025</div>
        <div class="record-body">
          <h3>Co-producer</h3>
          <p>Location Coordination · Short film <strong>《铜铃响了一整天》</strong></p>
          <p>Liangshan Yi Autonomous Prefecture</p>
          <p>
            I coordinated filming permissions and locations, local crew and resources, transportation and accommodation, stakeholder communication, and
            on-site logistics and safety.
          </p>
        </div>
      </div>
      <div class="academic-record">
        <div class="record-date">Summer 2023</div>
        <div class="record-body">
          <h3>Sichuan-Tibet Cycling Journey</h3>
          <p>Long-distance cycling · route318, China</p>
          <p>
            I completed over 2,000 km of long-distance, high-altitude cycling along route318 in 21 days.
          </p>
        </div>
      </div>
    </section>

  </div>
</div>
