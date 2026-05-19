---
layout: page
title: The Shielding Effect
description: How workplace segregation can countervail occupational segregation
img: /assets/img/publication_preview/shielding-effect.svg
importance: 1
category: research
related_publications: false
---

**Co-authors:** Martin Arvidsson, Maria Brandén, Károly Takács
**Status:** Under R&R at *European Sociological Review* — full draft available on request.

## The puzzle

People tend to prefer working alongside colleagues who share their gender. The standard story says this preference drives **occupational segregation**: when a worker becomes a gender minority in their occupation, they leave, the occupation tips further, and so on. So gender-mixed workplaces should help, while gender-sorted workplaces should make things worse.

Our paper argues the opposite can be true. **Workplaces sorted by gender can *shield* minorities from the pressure to exit their occupation.** A woman who is a numerical minority in her field of work may nevertheless sit on a team that is mostly women — and that local pocket meets her preference well enough that she stays. The net effect is that workplace segregation *dampens*, rather than reinforces, occupational segregation.

The effect is structurally asymmetric: shielding works mainly by keeping occupational *minorities* in place, with little offsetting effect on the majority — so it does not cancel out in the aggregate.

## Try it

The simulation below runs two synthetic labour markets side by side. Workers, preferences, and occupations are identical in both — the only difference is whether workplaces *within* each occupation are gender-mixed or gender-sorted. The shaded band in the chart is the **shielding effect**: the gap between occupational segregation in the integrated-workplace world and in the sorted-workplace world.

Sliders let you change homophily strength (α) and how much workplace versus occupational composition matters in the choice (η). The full agent-based model and parameter values are described in the paper's SI-1.

<div class="simulation-embed">
  <iframe src="{{ '/assets/html/shielding-effect-simulation.html' | relative_url }}"
          title="Shielding effect — interactive simulation"
          loading="lazy"
          allowfullscreen></iframe>
</div>

## Data and methods

The paper itself is empirical: we use **Swedish full-population register data** linking individuals to their occupation and workplace over time. The simulation above is a stylised illustration of the mechanism we identify in the data.
