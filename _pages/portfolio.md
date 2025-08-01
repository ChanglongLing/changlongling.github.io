---
title: "Portfolio"
permalink: /portfolio/
---

<style>
.project-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 2em;
  justify-content: center;
  align-items: flex-start;
  margin-top: 1em;
}

.project-card {
  width: 300px;
  text-align: center;
  position: relative;
  box-sizing: border-box;
  font-family: var(--global-font-family, 'Raleway', sans-serif);
  color: var(--global-text-color, #333);
  background-color: transparent;
  border-radius: 10px;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}
.project-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.12);
}
html[data-theme="dark"] .project-card:hover {
  box-shadow: 0 4px 14px rgba(255, 255, 255, 0.05);
}

.project-card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 10px;
  border: 1px solid #ddd;
}

.project-title {
  font-weight: 600;
  margin-top: 0.6em;
  font-size: 1.1rem;
  letter-spacing: 0.02em;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  user-select: none;
  color: var(--global-text-color, #222);
}
html[data-theme="dark"] .project-title {
  color: var(--global-text-color, #eee);
}

.toggle-arrow {
  font-size: 1em;
  margin-left: 0.4em;
  transition: transform 0.2s;
}
.project-title .toggle-arrow.open {
  transform: rotate(90deg);
}

.project-desc {
  color: var(--global-text-color-light, #666);
  margin-top: 0.3em;
  font-size: 0.95rem;
  max-height: 0;
  overflow: hidden;
  opacity: 0;
  line-height: 1.6;
  transition: max-height 0.25s, opacity 0.18s;
}
.project-desc.open {
  max-height: 260px;
  opacity: 1;
  margin-bottom: 0.5em;
}
html[data-theme="dark"] .project-desc {
  color: var(--global-text-color-light, #bbb);
}
</style>


<div class="project-grid">

  <div class="project-card">
    <a href="https://doi.org/10.1016/j.jtrangeo.2024.103820" target="_blank">
      <img src="/images/portfolio/exce_comm.jpg" alt="Excess Commuting">
    </a>
    <div class="project-title" onclick="toggleDesc(this)">
      Disaggregated Excess Commuting
      <span class="toggle-arrow" aria-hidden="true">
        <svg width="18" height="18" viewBox="0 0 18 18">
          <polyline points="4,7 9,12 14,7" fill="none" stroke="#888" stroke-width="2"/>
        </svg>
      </span>
    </div>
    <div class="project-desc">
      How much can cities reduce commutes by adopting more efficient layouts? This study developed a disaggregated excess commuting framework to measure the efficiencies by industry sectors using commute location-based service big data.
    </div>
  </div>

  <div class="project-card">
    <a href="https://doi.org/10.1038/s44333-024-00013-5" target="_blank">
      <img src="/images/portfolio/tce_tcf.jpg" alt="Transportation Emission">
    </a>
    <div class="project-title" onclick="toggleDesc(this)">
      Transportation Carbon Emission & Footprint
      <span class="toggle-arrow" aria-hidden="true">
        <svg width="18" height="18" viewBox="0 0 18 18">
          <polyline points="4,7 9,12 14,7" fill="none" stroke="#888" stroke-width="2"/>
        </svg>
      </span>
    </div>
    <div class="project-desc">
      It's often confusing when using the interconnected concepts of transportation carbon emission and footprint. The study delves into a large number of literature and draw comparisons between them to clarify their natures.
    </div>
  </div>

  <div class="project-card">
    <img src="/images/portfolio/sdk_gd.jpg" alt="Regional Mobility">
    <div class="project-title" onclick="toggleDesc(this)">
      Regional Mobility Networks
      <span class="toggle-arrow" aria-hidden="true">
        <svg width="18" height="18" viewBox="0 0 18 18">
          <polyline points="4,7 9,12 14,7" fill="none" stroke="#888" stroke-width="2"/>
        </svg>
      </span>
    </div>
    <div class="project-desc">
      How are cities funcationally connected? This study applies a mobility big data-driven approach and re-defines the metropolitan areas using location-based service big data.
    </div>
  </div>

  <div class="project-card">
    <img src="/images/portfolio/heyuan.jpg" alt="Transportation">
    <div class="project-title" onclick="toggleDesc(this)">
      Transportation Planning
      <span class="toggle-arrow" aria-hidden="true">
        <svg width="18" height="18" viewBox="0 0 18 18">
          <polyline points="4,7 9,12 14,7" fill="none" stroke="#888" stroke-width="2"/>
        </svg>
      </span>
    </div>
    <div class="project-desc">
      This project develops city-level strategic plans of comprehensive transportation systems, including roads, railway, airports, and water transportation as a part of the city master planning.
    </div>
  </div>

  <div class="project-card">
    <img src="/images/portfolio/jiangdong.jpg" alt="Traffic Safety">
    <div class="project-title" onclick="toggleDesc(this)">
      Improving Traffic Safety
      <span class="toggle-arrow" aria-hidden="true">
        <svg width="18" height="18" viewBox="0 0 18 18">
          <polyline points="4,7 9,12 14,7" fill="none" stroke="#888" stroke-width="2"/>
        </svg>
      </span>
    </div>
    <div class="project-desc">
      This project proposes road redevelopment and traffic light management strategies to address the problems faced by fast-urbanizing new town areas of Heyuan City. Local solutions have been developed and piloted to mitigate conflicts arising from fast land development, increasing traffic demand, and the shortage of road capacity.
    </div>
  </div>

  <div class="project-card">
    <a href="http://wupen.org/competitions/17?type=award" target="_blank">
      <img src="/images/portfolio/covid-survey.jpg" alt="COVID 2020">
    </a>
    <div class="project-title" onclick="toggleDesc(this)">
      WUPEN Survey 1st Prize
      <span class="toggle-arrow" aria-hidden="true">
        <svg width="18" height="18" viewBox="0 0 18 18">
          <polyline points="4,7 9,12 14,7" fill="none" stroke="#888" stroke-width="2"/>
        </svg>
      </span>
    </div>
    <div class="project-desc">
      Surveying twenty two COVID-19 patients in depth to explore what constrained their medical-service-seeking behavior and how the interaction worked in February to April 2020 in Wuhan, China.
    </div>
  </div>

  <div class="project-card">
    <a href="http://www.yuanyebei.com/index.php?m=YuanYeBei&a=index_show&contentid=276278&r=all" target="_blank">
      <img src="/images/portfolio/yuanye20.jpg" alt="Yuanye Cup 2020">
    </a>
    <div class="project-title" onclick="toggleDesc(this)">
      YUANYE Cup 2nd Prize
      <span class="toggle-arrow" aria-hidden="true">
        <svg width="18" height="18" viewBox="0 0 18 18">
          <polyline points="4,7 9,12 14,7" fill="none" stroke="#888" stroke-width="2"/>
        </svg>
      </span>
    </div>
    <div class="project-desc">
      Redeveloping old towns for living with animals -- "The cranes are crying in the marshes, and their voices are heard in the wilds", a wisdom from ancient Chinese literature <i>Xiaoya, Shijing</i>. We use the modern Community of Life theory to implement this vision and organize the environmental planning and urban redevelopment.
    </div>
  </div>

  <div class="project-card">
    <img src="/images/portfolio/comm_cent.jpg" alt="Community Center">
    <div class="project-title" onclick="toggleDesc(this)">
      Community Center Design
      <span class="toggle-arrow" aria-hidden="true">
        <svg width="18" height="18" viewBox="0 0 18 18">
          <polyline points="4,7 9,12 14,7" fill="none" stroke="#888" stroke-width="2"/>
        </svg>
      </span>
    </div>
    <div class="project-desc">
      Planning for livable communities with strong cultural symbols. Combining green building technologies with site-dependent spatial forms, the community center aims to reshape activities within the space and beyond.
    </div>
  </div>

</div>


<script>
function toggleDesc(titleElem) {
  const card = titleElem.parentElement;
  const desc = card.querySelector('.project-desc');
  const arrow = titleElem.querySelector('.toggle-arrow');
  desc.classList.toggle('open');
  arrow.classList.toggle('open');
}
</script>
