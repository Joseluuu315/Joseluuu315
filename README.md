<div align="center">

# José Luis Fuentes Parra

### Full-Stack Developer · Software Architect

**I build production SaaS that businesses run their day on** — multi-tenant ERP/CRM,
fiscal compliance, and the unglamorous reliability work in between.

<p>
  <a href="https://averonix.org"><img src="https://img.shields.io/badge/Portfolio-averonix.org-111111?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/jos%C3%A9-luis-fuentes-parra-80bb96257/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:joselufupa2016@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://wakatime.com/@b0a5de9a-56ed-4348-8790-cc98ac53626f"><img src="https://img.shields.io/badge/WakaTime-000000?style=for-the-badge&logo=wakatime&logoColor=white" alt="WakaTime"></a>
</p>

<p>
  <img src="https://img.shields.io/badge/Based%20in-Spain%20%C2%B7%20CET-4C9A2A?style=flat-square" alt="Based in Spain, CET timezone">
  <img src="https://img.shields.io/badge/Languages-ES%20%C2%B7%20CA%20%C2%B7%20EN-4C9A2A?style=flat-square" alt="Spanish, Catalan, English">
  <img src="https://img.shields.io/badge/Open%20to-Remote%20%26%20Hybrid-4C9A2A?style=flat-square" alt="Open to remote and hybrid">
</p>

</div>

---

## About

**Head Developer at [DGTalit](https://www.dgtalit.com/)**, where I lead a multi-tenant ERP/CRM SaaS running in
production for real client companies: invoicing with Spanish **VeriFactu** tax compliance, CRM pipelines and
quoting, project and ticket management, queued background jobs, and a trilingual interface (ES / EN / CA).

What I actually spend my time on:

- **Tenant isolation and authorisation.** Every data path answers one question first: can a user of tenant A
  reach tenant B through here? Session-derived scoping, server-side permission checks, immutable audit trails.
- **Change that does not break what works.** Additive-only schemas, backwards-compatible APIs, migrations that
  cannot lose a row, and a rollback plan written before the deploy rather than after it.
- **Regulated and financial data.** Spanish e-invoicing (VeriFactu), money as integers in cents, UTC-first
  timestamps, GDPR / LOPDGDD data subject rights, soft deletes over destructive ones.
- **Shipping without a safety net.** Direct-to-production deploys on self-managed VPS infrastructure, which is
  excellent training in caring about the thing before you push it.

Currently going deeper into **LLM integration inside business software** and **web application security**.

---

## Tech Stack

| | |
| :--- | :--- |
| **Languages** | ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white) ![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) |
| **Frontend** | ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white) ![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white) ![Tailwind](https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white) |
| **Backend** | ![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white) ![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=spring&logoColor=white) ![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white) ![BullMQ](https://img.shields.io/badge/BullMQ-DC382D?style=flat-square&logo=redis&logoColor=white) |
| **Data** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite%20%2F%20LibSQL-003B57?style=flat-square&logo=sqlite&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) |
| **Infra & Tooling** | ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![PM2](https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white) |

---

## Featured Work

### Portal DGTALIT — Multi-Tenant ERP/CRM SaaS

*Lead developer · running in production · private repository*

A full business operations platform used by client companies to run quoting, invoicing, CRM, projects and
support from one place.

- **Multi-tenant by construction** — every query scoped from the session; a valid ID from another tenant
  returns 404, never someone else's data
- **Spanish VeriFactu e-invoicing** — per-company tax identity, atomic document sealing, certificate expiry
  warnings
- **40+ data models and 40+ API routes**, strict TypeScript end to end
- **Async by default** — queued workers for email, imports, exports and reports, so the request path stays fast
- **Trilingual** (ES / EN / CA) with full i18n coverage, down to `aria-label`s and validation messages

`Next.js 16` · `React` · `TypeScript` · `Prisma` · `LibSQL` · `NextAuth` · `BullMQ` · `Redis` · `TailwindCSS` · `PM2`

### Averonix — [averonix.org](https://averonix.org)

*Personal engineering site and project index*

<!--
  Add one or two more PUBLIC repositories here. Recruiters click pinned repos first,
  so a short, concrete entry beats a long list:

  ### Project Name — [repository](https://github.com/Joseluuu315/repo)
  *One line on what it does and who it is for*
  - The interesting technical decision
  - The constraint that made it hard
  `Stack` · `Stack`
-->

---

## Experience

| Role | Company | Focus |
| :--- | :--- | :--- |
| **Head Developer / Head Admin** | [DGTalit](https://www.dgtalit.com/) | Enterprise SaaS architecture, multi-tenant data isolation, fiscal compliance, production operations |
| **Full-Stack Developer** | Solventium | REST API design, relational data modelling, SQL systems |

---

## GitHub

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Joseluuu315&show_icons=true&theme=tokyonight&hide_border=true&border_radius=10&include_all_commits=true&count_private=true" alt="GitHub statistics">
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Joseluuu315&layout=compact&theme=tokyonight&hide_border=true&border_radius=10&langs_count=8&hide=html,css" alt="Most used languages">

<img height="165" src="https://streak-stats.demolab.com/?user=Joseluuu315&theme=tokyonight&hide_border=true&border_radius=10" alt="Contribution streak">

<img src="https://komarev.com/ghpvc/?username=Joseluuu315&label=Profile+views&color=0e76a8&style=flat-square" alt="Profile views">

</div>

---

## Let's Talk

I am open to conversations about **senior full-stack and backend roles**, **SaaS architecture**, and work where
data integrity actually matters.

<div align="center">

<a href="mailto:joselufupa2016@gmail.com"><img src="https://img.shields.io/badge/Email%20me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email me"></a>
<a href="https://www.linkedin.com/in/jos%C3%A9-luis-fuentes-parra-80bb96257/"><img src="https://img.shields.io/badge/Connect%20on%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn"></a>
<a href="https://averonix.org"><img src="https://img.shields.io/badge/See%20my%20work-111111?style=for-the-badge&logo=googlechrome&logoColor=white" alt="See my work"></a>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=100&section=footer" width="100%" alt="">
