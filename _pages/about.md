---
layout: about
title: about
permalink: /
subtitle: PhD candidate · <a href='https://liu.se/en/organisation/liu/iei/ias'>Institute for Analytical Sociology</a>, Linköping University.

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false
  more_info: >
    <p>Institute for Analytical Sociology</p>
    <p>Linköping University</p>
    <p>Norrköping, Sweden</p>

news: true
selected_papers: true
social: true
---

<p class="profile-lede">
I study how labour markets sort people into occupations — and why those sorts so reliably break along gender lines.
</p>

<dl class="profile-rows">
  <dt>Research</dt>
  <dd>Occupational gender segregation, studied with Swedish full-population register data and computational methods. A second strand: scholarly mobility and how collaboration networks shape researchers' opportunity space.</dd>

  <dt>Methods</dt>
  <dd>Social network analysis · agent-based modelling · NLP · register-data analytics</dd>

  <dt>Background</dt>
  <dd>MSc Social Data Science (<a href="https://www.oii.ox.ac.uk/">Oxford</a>) · MPP Public Policy (Berlin) · BSc Physics + Geography (Heidelberg)</dd>

  <dt>Supervised by</dt>
  <dd><a href="https://liu.se/en/employee/karta65">Károly Takács</a> · <a href="https://martin-arvidsson.github.io/">Martin Arvidsson</a></dd>

  <dt>Get in touch</dt>
  <dd><a href="mailto:alexandra.rottenkolber@liu.se">alexandra.rottenkolber@liu.se</a> · <a href="{{ '/assets/pdf/Rottenkolber_CV_Website.pdf' | relative_url }}">download CV (PDF)</a></dd>
</dl>

<p class="profile-offhours">
When I'm not coding, reading, or writing, I'm usually out on a lakeshore trail or tending to plants.
</p>

<!-- ============================================================
     Unfolding sections — CV, Talks, Teaching, Code.
     These render below the news block automatically because the
     about layout pushes the news + selected_papers blocks first.
     ============================================================ -->

<section class="more-sections" markdown="0">

<details id="cv">
  <summary>
    <span class="summary-text">
      Curriculum vitae
      <a class="cv-pdf-link"
         href="{{ '/assets/pdf/Rottenkolber_CV_Website.pdf' | relative_url }}"
         target="_blank" rel="noopener"
         onclick="event.stopPropagation()"
         title="Download CV as PDF"
         aria-label="Download CV as PDF">
        <i class="fa-solid fa-file-pdf"></i><span class="pdf-label">PDF</span>
      </a>
    </span>
  </summary>
  <div class="details-body">
    {% include cv_content.liquid %}
  </div>
</details>

<details id="talks">
  <summary><span class="summary-text">Selected talks &amp; presentations</span></summary>
  <div class="details-body">
    <p class="details-meta"><em>To be added.</em></p>
  </div>
</details>

<details id="teaching">
  <summary><span class="summary-text">Teaching</span></summary>
  <div class="details-body">
    <p class="details-meta"><em>To be added.</em></p>
  </div>
</details>

<details id="code">
  <summary><span class="summary-text">Code</span></summary>
  <div class="details-body">
    <p>Most of my code lives on GitHub —
      <a href="https://github.com/AlexandraRoko" target="_blank" rel="noopener">github.com/AlexandraRoko ↗</a>.
    </p>
  </div>
</details>

</section>

<script>
// Open the targeted <details> when the page is opened with a hash (e.g. /#cv),
// then re-scroll because opening changes the page height.
(function () {
  function handleHash() {
    var hash = window.location.hash;
    if (!hash || hash.length < 2) return;
    var el;
    try { el = document.querySelector(hash); } catch (e) { return; }
    if (!el) return;
    var details = el.closest ? el.closest('details') : null;
    if (details && !details.open) details.open = true;
    setTimeout(function () {
      el.scrollIntoView({ behavior: 'smooth', block: 'start' });
    }, 60);
  }
  window.addEventListener('hashchange', handleHash);
  window.addEventListener('load', handleHash);
})();
</script>
