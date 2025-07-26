---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! I'm **Changlong Ling**, a first-year PhD student in the [Interdisciplinary PhD Program in Urban Design and Planning](https://sites.uw.edu/urbdpphd/) at the **_University of Washington_**, where I am advised by Prof. [Qing Shen](https://urbdp.be.uw.edu/people/qing-shen/). I earned a master's degree in Urban Planning from Peking University and dual bachelor's degrees in Economics and Urban Planning from Wuhan University.

My research interests are in developing artificial intelligence (AI) algorithms and statistical/data science methods to support the integration of automated vehicles and digital technologies into urban mobility systems. I utilize responsible, explainable, and generative AI to enhance the economic effectiveness, systematic smartness, and environmental sustainability of future transportation, ultimately informing more equitable public policies. I have led several urban and transportation planning projects that were implemented in cities.

My current research topics include, but are not limited to:
- **Automated and Sustainable Transportation**: Autonomous Vehicles for Public Transit, Transportation Decarbonization & Traffic Safety
- **Digital Economy and Smart Cities**: Remote Work, Urban Sustainability, Transit-Oriented Development & Urban Networks
- **Machine Learning and Causal Inference**: Causal Machine Learning, Explainability, (Spatial) Econometrics & Optimization

I view planning as a collaborative endeavor and enjoy working with others to tackle real-world challenges. If you are interested in my work, feel free to reach out :)

News
-----
- **[Sep 2024]** Awarded [Hubert M. Blalock Fellowships](https://csss.uw.edu/about/blalock-fellowship) by the Center for Statistics and the Social Sciences (CSSS), University of Washington!
- **[Sep 2024]** New journey, PhD life, starts at the University of Washington!
- **[Jun 2024]** Graduated with distinction from Peking University!

---

<h2>📍 当前访客大致位置</h2>
<div id="map" style="height: 400px; margin-bottom: 2rem;"></div>

<!-- Leaflet 地图样式和脚本 -->
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.3/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet@1.9.3/dist/leaflet.js"></script>

<script>
// 获取 IP 位置
fetch("https://ipapi.co/json/")
  .then(response => response.json())
  .then(data => {
    const lat = data.latitude;
    const lon = data.longitude;
    const city = data.city;
    const country = data.country_name;

    // 初始化地图
    const map = L.map('map').setView([lat, lon], 10);
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      attribution: '&copy; OpenStreetMap contributors'
    }).addTo(map);

    // 添加 marker
    L.marker([lat, lon]).addTo(map)
      .bindPopup(`你大致位于：${city}, ${country}`)
      .openPopup();
  });
</script>
