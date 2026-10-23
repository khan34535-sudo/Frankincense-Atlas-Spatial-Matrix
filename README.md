# 🌿 Frankincense Atlas & Spatial Matrix (*Boswellia sacra*)

> **An interactive, multi-sensory 3D research dashboard mapping the geography, microclimatic terroir, scriptural history, commercial grades, and pharmacological profiles of Omani *Boswellia sacra*.**

![Copyright](https://img.shields.io/badge/Copyright-All_Rights_Reserved-gold.svg)
![Build: Zero--Dependency](https://img.shields.io/badge/Architecture-Zero--Backend-00f0ff.svg)
![WebGL: Three.js](https://img.shields.io/badge/3D_Engine-Three.js_r128-2ecc71.svg)
![GIS: Leaflet](https://img.shields.io/badge/GIS-Leaflet_v1.9-9b59b6.svg)

---

## 📌 Executive Summary

The **Frankincense Atlas & Spatial Matrix** bridges paleoethnobotany, phytochemistry, spatial GIS mapping, and 3D WebGL visualization into a unified, client-side digital twin. Developed by **Asia Khan**, this application explores how microclimate variations across Oman's Dhofar region directly dictate the resin chemistry, color, market grade, and pharmacological efficacy of *Boswellia sacra*.

---

## ✨ Key Features & Capabilities

* **🔶 3D Resin Grade Viewer & Terroir Analysis:**
  * Interactive WebGL renderer (Three.js) modeling organic resin teardrops.
  * Real-time material shader updates reflecting translucent colors, surface roughness, and light-refraction across the four primary commercial grades (*Royal Hojari*, *Najdi*, *Shathari*, and *Shaabi*).
  * Embedded GIS microclimate map detailing altitude, annual rainfall, and soil geology across Dhofar’s ecological harvesting zones.

* **🛰️ Tilted 3D Satellite GIS Map:**
  * Built on Leaflet.js with Esri World Imagery overlays.
  * Maps ancient trade caravans (the Incense Road through Sumhuram/Khor Rori, Ubar, Shabwa, Marib, Petra, and Gaza) against modern maritime export corridors.

* **👃 Olfactory Chemistry & Radar Comparison:**
  * Chart.js radar engine comparing GC-olfactometry datasets ($\alpha$-pinene, myrcene, limonene) across resin qualities.

* **🧪 Traditional-to-Clinical Health Matrix:**
  * Dual-layer clinical evidence mapping connecting traditional uses (Unani, Prophetic, and Ayurvedic) to modern pharmacological trials (boswellic acids, AKBA pathways, 5-LOX inhibition, and cytotoxic research).

* **⏳ Interactive Chronology & Scriptural Traditions:**
  * 13-era interactive timeline spanning 6000 BCE to 2026.
  * Primary textual analysis across Torah (*Ketoret*), New Testament (Magi), and Islamic traditions.

---

## 🛠️ Tech Stack & Architecture

This application is built using a **Zero-API, Client-Side Architecture** requiring no server-side compilation or backend infrastructure:

* **Core Engine:** HTML5, CSS3 (CSS Variables, Flexbox/Grid, Glassmorphism), Vanilla JavaScript (ES6+)
* **3D Graphics:** [Three.js (r128)](https://threejs.org/) + `OrbitControls`
* **Geospatial Mapping:** [Leaflet.js (v1.9.4)](https://leafletjs.com/) + Esri World Imagery Tiles
* **Data Visualization:** [Chart.js (v4.4.1)](https://www.chartjs.org/)
* **Typography:** Google Fonts (`Cinzel`, `Plus Jakarta Sans`, `Orbitron`)

---

## 🚀 Quick Start

Because the project is entirely self-contained, no `npm install` or local server build step is required.

🔒 Copyright & Intellectual Property
Copyright © 2026 Asia Khan. All Rights Reserved.

This repository, including all code, custom WebGL shaders, visual design assets, curated dataset matrices, and spatial architecture, is the exclusive intellectual property of Asia Khan.

No part of this software, code, or content may be reproduced, distributed, modified, sublicensed, or transmitted in any form or by any means (electronic, mechanical, photocopying, recording, or otherwise) without prior explicit written permission from the copyright owner.

📚 Academic Citation & Bibliography (APA 7th)
When referencing this research or software implementation in academic or museum contexts, please cite:

Al-Harrasi, A., Al-Rawahi, A., & Khan, A. L. (2019). Biology of Genus Boswellia. Springer Nature.

Groom, N. (1981). Frankincense and Myrrh: A Study of the Arabian Incense Trade. Longman.

Moussaieff, A., & Mechoulam, R. (2009). Boswellia resin: From religious ceremonies to medical uses; a review of in-vitro and in-vivo studies. Journal of Pharmacy and Pharmacology, 61(10), 1281–1293.

UNESCO World Heritage Centre. (2000). Land of Frankincense (Wadi Dawkah, Shisr, Khor Rori, Al-Baleed). UNESCO Cultural Heritage List No. 1010.

👤 Author & Contact
Asia Khan

Behavioural UX Researcher & 3D Spatial Architect

Hon. BA, McMaster University

📧 Email: asiaaamirkhan@outlook.com

https://khan34535-sudo.github.io/Frankincense-Atlas-Spatial-Matrix/
