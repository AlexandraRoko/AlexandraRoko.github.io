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

I study how labour markets sort people into occupations — and why those sorts so reliably break along gender lines. My dissertation uses Swedish full-population register data and computational methods to get at the mechanisms behind occupational gender segregation. A second strand of my work looks at scholarly mobility: how a researcher's personal and institutional embedding shapes the opportunity space they move through.

I'm a trained social data scientist ([Oxford](https://www.oii.ox.ac.uk/)) with earlier degrees in public policy (Berlin) and physics and geography (Heidelberg). My past projects combined NLP, social network analysis, and agent-based modelling to study policymaking in the German parliament, how nations digitize over time, and how gender shapes online interaction.

I'm supervised by [Károly Takács](https://liu.se/en/employee/karta65) and [Martin Arvidsson](https://martin-arvidsson.github.io/).

When I'm not coding, reading, or writing, I'm usually out on a lakeshore trail or tending to plants. You can [download my CV](/assets/pdf/Rottenkolber_CV_Website.pdf) or reach me at <a href="mailto:alexandra.rottenkolber@liu.se">alexandra.rottenkolber@liu.se</a>.

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
  <summary>Selected talks &amp; presentations</summary>
  <div class="details-body">
    <p class="details-meta"><em>To be added.</em></p>
  </div>
</details>

<details id="teaching">
  <summary>Teaching</summary>
  <div class="details-body">
    <p class="details-meta"><em>To be added.</em></p>
  </div>
</details>

<details id="code">
  <summary>Code</summary>
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
