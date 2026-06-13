---
layout: about
title: About
permalink: /
subtitle: Embodied Co-Design · Robotics · Agentic Systems

profile:
  align: left
  image: bio_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
      <a href="mailto:wyx20@mails.tsinghua.edu.cn" title="Email"><i class="fa-solid fa-square-envelope fa-2x"></i></a>
      <a href="/assets/pdf/YW_Resume.pdf"><i class="ai ai-cv-square ai-2x"></i></a>
      <a href="https://www.linkedin.com/"><i class="fa-brands fa-linkedin fa-2x"></i></a>
      <a href="https://scholar.google.com/citations?user=ac-6jfMAAAAJ"><i class="ai ai-google-scholar-square ai-2x"></i></a>
      <a href="https://github.com/Yuxing-Wang-THU"><i class="fa-brands fa-square-github fa-2x"></i></a>
      <a href="/assets/img/wechat-qr.png"><i class="fa-brands fa-weixin fa-2x"></i></a>

news: true # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
awards: true
social: false # includes social icons at the bottom of the page

---
<section class="academic-hero">
  <div class="hero-portrait">
    <img src="/assets/img/bio_pic.jpg" alt="Yuxing Wang portrait">
    {% if page.profile.more_info %}
      <div class="portrait-links">{{ page.profile.more_info }}</div>
    {% endif %}
  </div>
  <div class="hero-copy">
    <p class="eyebrow">您好 · Привет · Hello · Bonjour · Ciao · こんにちは · 안녕하세요 · Hallo · Hola</p>
    <h4>Designing machines that design machines.</h4>
    <p class="lead">
      I am <strong>Yuxing Wang</strong>, a researcher working on
      <strong>Embodied Co-Design</strong>, <strong>Robot Learning</strong>, and Agentic AI.
    </p>
    <p class="hero-bio">
      My work is driven by a fascination with systems that can move, adapt, and eventually participate in their own design.
      I study how learning algorithms, physical morphology, and environmental structure can be optimized together, so embodied agents are not only structurally feasible but behaviorally capable.
    </p>
    <figure class="concept-figure">
      <img src="/assets/img/machine-design-loop.png" alt="Cartoon illustration of a robot design loop">
    </figure>
    <!-- <div class="hero-actions">
      <a class="btn btn-primary btn-sm" href="/publications/">Publications</a>
      <a class="btn btn-outline-primary btn-sm" href="https://github.com/Yuxing-Wang-THU">GitHub Projects</a>
      <a class="btn btn-outline-primary btn-sm" href="/assets/pdf/YW_Resume.pdf">CV</a>
    </div> -->
  </div>
</section>

<section class="about-grid">
  <div class="about-card">
    <h3>Biography</h3>
    <p>
      I earned my B.Eng. from <a href="https://www.swun.edu.cn/">Southwest Minzu University</a> in 2020
      and my M.Eng. from <a href="https://www.tsinghua.edu.cn/">Tsinghua University</a> in 2023, advised by
      <a href="https://scholar.google.com/citations?user=h9dN_ykAAAAJ&hl=zh-CN">Prof. Xueqian Wang</a>.
      I am now pursuing a Ph.D. in Control Science and Engineering at Tsinghua.
    </p>
    <p>
      During my 2022-2023 research internship at <a href="https://ai.tencent.com/ailab/">Tencent AI Lab</a>,
      supported by the Tencent Rhino-Bird Research Elite Program, I worked with
      <a href="https://scholar.google.com/citations?hl=zh-CN&user=_MtBmxkAAAAJ">Shuang Wu</a> and
      <a href="https://haobofu.github.io/">Haobo Fu</a> on user-specified behavioral diversity for Game AI.
    </p>
  </div>
  <div class="about-card accent-card">
    <h3>Research Style</h3>
    <p>
      I like research that is visual, physical, and a little stubborn: systems should move, fail, improve,
      and eventually reveal a design principle.
    </p>
    <p>Outside the lab, I recharge with
      <a href="https://en.wikipedia.org/wiki/Hikaru_Utada">Hikaru Utada</a>, comedies, and talk shows.
    </p>
  </div>
</section>

{% if page.news and site.announcements.enabled %}
<section class="home-news-section">
  <div class="section-kicker"><a href="{{ '/news/' | relative_url }}">News</a></div>
  {% include news.liquid limit=true %}
</section>
{% endif %}

<section class="report-section">
  <div class="section-kicker">Report</div>
  <a class="report-card" href="https://www.mittrchina.com/news/detail/15865">
    <div>
      <h3>MIT Technology Review China coverage</h3>
      <p>我设计我自己！清华最新研究：未来机器人不用人设计，AI直接捏出最优形态</p>
    </div>
    <span>Read report</span>
  </a>
</section>

<section class="featured-work">
  <div class="section-kicker">Selected Works</div>
  <div class="work-strip">
    <a class="work-card" href="https://github.com/Yuxing-Wang-THU/ModularEvoGym">
      <img src="/assets/img/modu.jpg" alt="ModularEvoGym preview">
      <div>
        <h3>ModularEvoGym</h3>
        <p>A co-design benchmark and methods for modular soft robot morphology and control.</p>
      </div>
    </a>
    <a class="work-card" href="https://github.com/Yuxing-Wang-THU/SurveyBrainBody">
      <img src="/assets/img/publication_preview/cover.jpg" alt="Embodied co-design survey preview">
      <div>
        <h3>SurveyBrainBody</h3>
        <p>A living survey on taxonomy, frontiers, and challenges in embodied co-design.</p>
      </div>
    </a>
    <a class="work-card" href="https://github.com/Yuxing-Wang-THU/Surrogate-assisted-ERL">
      <img src="/assets/img/serl.jpg" alt="Surrogate-assisted ERL preview">
      <div>
        <h3>Surrogate-assisted ERL</h3>
        <p>Reducing expensive controller search with learned fitness estimation.</p>
      </div>
    </a>
  </div>
</section>
