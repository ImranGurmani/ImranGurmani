<!-- ======================================================== -->
<!-- Imran Khan Gurmani (Jigar Gurmani) - GitHub Profile README -->
<!-- Palette: Obsidian Dark (#08080C) + Luxury Neon Gold (#FACC15) -->
<!-- Generated for: https://imrangurmani.shop -->
<!-- ======================================================== -->

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=08080c&height=220&section=header&text=Imran%20Khan%20Gurmani&fontSize=42&fontColor=FACC15&fontAlignY=40&desc=Full-Stack%20Architect%20%7C%20AI%20Ventures%20%7C%20Digital%20Entrepreneur&descColor=A1A1AA&descAlignY=62" width="100%" />
</div>

<p align="center">
  <a href="https://imrangurmani.shop"><img src="https://img.shields.io/badge/Portfolio-imrangurmani.shop-FACC15?style=for-the-badge&logo=google-chrome&logoColor=000&labelColor=08080c" alt="Portfolio" /></a>
  <a href="mailto:contact@imrangurmani.shop"><img src="https://img.shields.io/badge/Email-Get_in_Touch-FFE249?style=for-the-badge&logo=gmail&logoColor=000&labelColor=08080c" alt="Email" /></a>
  <a href="https://github.com/imrangurmani"><img src="https://img.shields.io/badge/Location-Kot%20Addu%2C%20Pakistan-FACC15?style=for-the-badge&logo=location-dot&logoColor=FACC15&labelColor=08080c" alt="Location" /></a>
</p>

<p align="center">
  <strong>"Crafting scalable code, mission-critical SaaS, and next-generation speech tech."</strong><br>
  Known across the developer web as <em>Jigar Gurmani</em>
</p>

---

### ⚡ Operational Telemetry & Metrics

- 🚀 **Projects Completed:** 50+ Production web apps, SaaS panels & APIs.
- 🤝 **Client Success:** 30+ Happy clients worldwide with 100% satisfaction.
- ⚡ **SaaS Uptime:** 99.9% uptime track record across high-volume platforms.
- 🎓 **GenXEmpire:** Trained 100+ students in full-stack engineering & AI workflows.
- 📍 **Base:** Kot Addu, Punjab, Pakistan.

---

### 🛸 Flagship Ventures & Ecosystem

| Platform | Core Domain | Technology Stack |
| :--- | :--- | :--- |
| **[SynVoice.io](https://synvoice.io)** | AI Voice Cloning & Speech Synthesis Platform | Python, XTTS-v2, StyleTTS 2, Astro JS, Tailwind |
| **[GeoSMM.pk](https://geosmm.pk)** | High-Traffic SMM Automation & Reseller API Gateway | PHP 8.2, MySQL High-Perf, Webhooks, Cron Queues |
| **[GenXEmpire.com](https://genxempire.com)** | AI Automation Academy & LMS Community | Astro JS, Tailwind CSS, Member Gating, Payments |
| **[MicroSmartLoan.in](https://microsmartloan.in)** | Complete Loan Management CRM & Installment Tracker | PHP, MySQL, Financial Math Engine, RBAC |
| **[RenZoify](https://renzoify.com)** | Bespoke Software Development & Web Agency | Full-Stack Modern Web, Custom CMS, UI/UX |

---

### 🛠️ Tech Arsenal & Stack

\`\`\`yaml
Languages:     PHP (8.x), JavaScript (ES6+), Python, SQL, HTML5/CSS3
Frameworks:    Astro JS, Node.js, Express, Tailwind CSS
Databases:     MySQL, MariaDB, Supabase, Redis
AI / Speech:   XTTS-v2, StyleTTS 2, Gemini API, ChatGPT / OpenAI APIs
Tooling:       Cursor AI, Roo Code, VS Code, Git/GitHub, Cloudflare, Linux Bash
\`\`\`

---

### 📊 GitHub Activity & Golden Telemetry

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=imrangurmani&show_icons=true&title_color=FACC15&text_color=D4D4D8&icon_color=FACC15&bg_color=08080c&border_color=27273a&hide_border=false" width="49%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=imrangurmani&theme=dark&background=08080c&border=27273a&stroke=FACC15&ring=FACC15&fire=FACC15&currStreakNum=FACC15&sideNums=EAB308&currStreakLabel=FACC15&dates=A1A1AA" width="49%" />
</div>

<br>

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=imrangurmani&layout=compact&title_color=FACC15&text_color=D4D4D8&bg_color=08080c&border_color=27273a&hide_border=false" />
</div>

---

### 🐍 GitHub Contribution Snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/imrangurmani/imrangurmani/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/imrangurmani/imrangurmani/output/github-contribution-grid-snake.svg">
  <img alt="github contribution grid snake" src="https://raw.githubusercontent.com/imrangurmani/imrangurmani/output/github-contribution-grid-snake.svg">
</picture>

---

<p align="center">
  <em>Designed with pride for <strong>Imran Khan Gurmani (Jigar Gurmani)</strong> • <a href="https://imrangurmani.shop">imrangurmani.shop</a></em>
</p>
`;

    // 6. Modal Functions
    const modal = document.getElementById("readmeModal");
    const markdownArea = document.getElementById("markdownArea");
    const toast = document.getElementById("toast");
    const copyBtnLabel = document.getElementById("copyBtnLabel");

    markdownArea.value = customizedReadmeMarkdown;

    function openReadmeModal() {
      modal.classList.remove("hidden");
    }

    function closeReadmeModal() {
      modal.classList.add("hidden");
    }

    modal.addEventListener("click", (e) => {
      if (e.target === modal) closeReadmeModal();
    });

    function showToastNotification() {
      toast.classList.remove("translate-y-20", "opacity-0");
      setTimeout(() => {
        toast.classList.add("translate-y-20", "opacity-0");
      }, 3500);
    }

    function copyMarkdownText() {
      const tempTextArea = document.createElement("textarea");
      tempTextArea.value = customizedReadmeMarkdown;
      document.body.appendChild(tempTextArea);
      tempTextArea.select();
      try {
        document.execCommand('copy');
        showToastNotification();
        copyBtnLabel.textContent = "Copied!";
        setTimeout(() => {
          copyBtnLabel.textContent = "Copy All Code";
        }, 2500);
      } catch (err) {
        console.error("Copy failed", err);
      }
      document.body.removeChild(tempTextArea);
    }
  </script>
</body>
</html>
