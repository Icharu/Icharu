---
date: 2026-05-17
type: profile
tags: [github, profile, readme, personal-brand]
aliases: [GitHub README, profile README, Icharu profile]
---

# GitHub profile README — `Icharu/Icharu`

> Source of truth for the README on my GitHub profile (`github.com/Icharu`). The vault stores it so I can keep iterating without losing history.
>
> ⚠️ **Before pushing to GitHub**, strip the YAML frontmatter block at the very top of this file (everything between the `---` lines). GitHub renders frontmatter as a small literal code block, which looks broken.
>
> **Placeholders to swap in before pushing:**
> - `<your-laps-repo>` (×2) — the actual repo URL for the LAPS frontend / backend.
> - Snake animation workflow — copy the YAML block at the bottom into `.github/workflows/snake.yml` of the `Icharu/Icharu` repo.

Related:
- [[00-PROJECTS]] — full project list this README distills from
- [[01-projects/laps/laps]] — LAPS project hub (the featured project)
- [[01-projects/laps/laps-graph-explainer]] — referenced from the LAPS card
- [[icaro_second_brain]] — personal-brand context

---

<!-- ════════════════════════════════════════════════════════════════════════ -->
<!-- EVERYTHING BELOW THIS LINE GETS COPIED INTO Icharu/Icharu/README.md      -->
<!-- ════════════════════════════════════════════════════════════════════════ -->

<!-- HEADER BANNER -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,2,30&height=200&section=header&text=Ícaro%20de%20Jesus&fontSize=58&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Computer%20Engineering%20·%20UEMA%20Researcher%20·%20PT%20·%20EN%20·%20FR&descAlignY=60&descSize=14" alt="header" />
</p>

<!-- ANIMATED TYPING SUBTITLE -->
<p align="center">
  <a href="https://github.com/Icharu">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2800&pause=900&color=22C55E&center=true&vCenter=true&width=720&lines=Building+reliable+systems+for+ecological+research;Spring+Boot+%2B+TanStack+%2B+TypeScript+full-stack;Trilingual+%F0%9F%87%A7%F0%9F%87%B7+%F0%9F%87%AC%F0%9F%87%A7+%F0%9F%87%AB%F0%9F%87%B7;Currently+working+at+Reserva+Biológica+do+Gurupi" alt="typing" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/Icharu"><img src="https://komarev.com/ghpvc/?username=Icharu&label=Profile%20views&color=22c55e&style=flat-square" alt="views" /></a>
  <a href="https://github.com/Icharu?tab=followers"><img src="https://img.shields.io/github/followers/Icharu?label=Followers&style=flat-square&color=22c55e" alt="followers" /></a>
</p>

---

## 👋 Introduction

Howdy! I am a **Computer Engineering student** from **São José de Ribamar, Maranhão, Brazil**, fluent in **Portuguese**, **English**, and **French** — always eager to find new strategic points to build scalable, consistent, and reliable applications.

My passion for web development and systems became clear after joining college, where I also took on a role as a **scientific researcher at UEMA** (Universidade Estadual do Maranhão).

Today, I am actively developing systems for **ecological research** at the **Reserva Biológica do Gurupi** — the only biological reserve in northeastern Brazil — applying software engineering to support the integrity and consistency of environmental data.

Interested in any of my projects? Check below for more info!

---

## 🚀 Featured Project — LAPS

> Full-stack platform for the **Laboratório de Aquisição e Processamento de Sinais** at UEMA. Public site, researcher network visualization, manager dashboard, and member portal — all backed by a single Spring Boot API.

<table>
  <tr>
    <td valign="top" width="50%">

**🧩 Highlights**
- 🎨 Interactive **researcher constellation** on `/team` — seeded-random anchors, draggable nodes with spring-back, pan + cursor-anchored zoom, tier-cascade hover (head ↔ doctorate ↔ master ↔ undergrad)
- 🌐 **Tri-lingual public site** (PT / EN / FR) with live-switching i18n via `useSyncExternalStore` — no page reloads
- 🤖 **Auto-translation pipeline** — managers write Portuguese bios; backend fills EN/FR through the MyMemory API on save
- 🔐 **JWT-cookie auth** (`SameSite=Lax`, HttpOnly), with MANAGER-gated `/admin/**` endpoints and an audit log on every mutation
- 📷 **Photo-upload pipeline** — multipart endpoint, UUID-named files served from `/uploads/**`, path-traversal-safe
- 🔍 **Searchable researcher picker** — deps-free weighted-score matcher (word-prefix + substring + initials + slug + email) over the live roster

</td>
<td valign="top" width="50%">

**🛠️ Stack**

| Layer | Tech |
|---|---|
| Backend | Java 21 · Spring Boot 3.4 · Spring Security · JPA · Flyway |
| Database | MySQL 8 |
| Frontend | React 18 · TanStack Start · TanStack Router · TanStack Query · TypeScript · Vite |
| Visuals | framer-motion · Canvas2D (Langevin dynamics for the hero) · SVG (constellation) |
| Tooling | Maven · Bun · Cloudflare Workers · TailwindCSS · shadcn/ui |

</td>
  </tr>
</table>

<sub>📂 Code & write-up: [Frontend](https://github.com/Icharu/<your-laps-repo>) · [Backend](https://github.com/Icharu/<your-laps-repo>) — for the deep dive (Langevin physics for the hero mesh, seeded-random layout for the constellation, framer-motion spring-back math), see the in-repo `laps-graph-explainer.md`.</sub>

---

## 🧠 Knowledge

### Backend
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=spring-security&logoColor=white)
![JPA / Hibernate](https://img.shields.io/badge/JPA_/_Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white)

### Frontend
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TanStack](https://img.shields.io/badge/TanStack-FF4154?style=for-the-badge&logo=react-query&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### Databases
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)

---

## 🔬 Current Focus

> Building data management systems for ecological and biodiversity research at the **Reserva Biológica do Gurupi**, northeastern Brazil.

- 🌿 Ecological data systems with a focus on **data integrity** and **observation provenance**
- 🎓 Scientific research at **UEMA** — signal processing, applied AI, biodiversity informatics
- 🌐 Full-stack web development with **Java + Spring Boot + TypeScript** (Angular and React/TanStack)
- 🧪 Interested in **graph-based scientific visualization** — see the LAPS researcher constellation above

---

## 📊 Status

<p align="center">
  <a href="https://git.io/streak-stats">
    <img src="https://streak-stats.demolab.com?user=Icharu&theme=dark&background=0d1117&border=30363d&ring=22c55e&fire=22c55e&currStreakLabel=22c55e&hide_border=true" alt="streak" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/anuraghazra/github-readme-stats">
    <img height="170" src="https://github-readme-stats.vercel.app/api?username=Icharu&show_icons=true&theme=github_dark&hide_border=true&icon_color=22c55e&title_color=22c55e&count_private=true" alt="stats" />
  </a>
  <a href="https://github.com/anuraghazra/github-readme-stats">
    <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Icharu&layout=compact&theme=github_dark&hide_border=true&title_color=22c55e&langs_count=8" alt="languages" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/Icharu">
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=Icharu&theme=github-compact&hide_border=true&color=22c55e&line=22c55e&point=ffffff&area=true" alt="contributions" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/ryo-ma/github-profile-trophy">
    <img src="https://github-profile-trophy.vercel.app/?username=Icharu&theme=darkhub&no-frame=true&no-bg=true&column=7&margin-w=8" alt="trophies" />
  </a>
</p>

---

## 🗣️ Languages

![Portuguese](https://img.shields.io/badge/Portuguese-Native-009C3B?style=for-the-badge&logo=googletranslate&logoColor=white)
![English](https://img.shields.io/badge/English-Fluent-012169?style=for-the-badge&logo=googletranslate&logoColor=white)
![French](https://img.shields.io/badge/French-Fluent-002395?style=for-the-badge&logo=googletranslate&logoColor=white)

---

## 🛠️ Workflow

![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=for-the-badge&logo=intellij-idea&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Bun](https://img.shields.io/badge/Bun-000000?style=for-the-badge&logo=bun&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)

---

## 🐍 Activity

<p align="center">
  <img src="https://raw.githubusercontent.com/Icharu/Icharu/output/github-contribution-grid-snake-dark.svg" alt="snake eating my contributions" />
</p>

> The snake graphic above is generated daily by the workflow at the bottom of this file. The first run pushes the SVG to an `output` branch, which the `<img>` tag above reads from.

---

## 🌐 Social — Network

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Icharu)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/icarodejesus/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/aliveicarus/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:icarodejesussilva3@gmail.com)

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,2,30&height=110&section=footer" alt="footer" />
</p>

<!-- ════════════════════════════════════════════════════════════════════════ -->
<!-- END OF GITHUB README CONTENT                                             -->
<!-- ════════════════════════════════════════════════════════════════════════ -->

---

## Snake animation workflow

Drop this YAML at `.github/workflows/snake.yml` in the `Icharu/Icharu` profile repo. After the first run the SVG lands on an `output` branch and the README's `<img>` tag picks it up automatically.

```yaml
name: generate snake
on:
  schedule: [{ cron: "0 */24 * * *" }]
  workflow_dispatch:
  push:
    branches: [main]

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk/svg-only@v3
        with:
          github_user_name: Icharu
          outputs: |
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark&color_snake=#22c55e&color_dots=#161b22,#22c55e,#16a34a,#15803d,#166534
      - uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

---

## Changelog

| Date | Change |
|---|---|
| 2026-05-17 | Initial enhanced version. Added animated capsule-render banner + typing SVG, profile-view counter, Featured Project (LAPS) card with stack table, expanded Knowledge section (Spring Security, JPA, Flyway, React, TanStack, Vite, Tailwind), activity graph + trophy display, snake animation, email badge, footer wave. Saved to vault for iteration. |
