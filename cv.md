---
title: Aliaksandr Dvaraninau — CV
description: Frontend Developer — Angular / TypeScript
---

# Aliaksandr Dvaraninau

![Aliaksandr Dvaraninau](https://github.com/assets/advoryan.jpg?size=240)

## Frontend Developer — Angular / TypeScript

---

## Contacts

- **Location:** Warsaw, Poland (open to relocate)
- **Phone:** [+48 452-594-320](tel:+48452594320)
- **E-mail:** [a.dvoryan@gmail.com](mailto:a.dvoryan@gmail.com)
- **LinkedIn:** [linkedin.com/in/a-dvaraninau](https://www.linkedin.com/in/a-dvaraninau/)
- **GitHub:** [github.com/advoryan](https://github.com/advoryan)
- **Telegram:** [@doubleJameson](https://t.me/doubleJameson)
- **Discord:** aDvoRyan

---

## About Me

Angular-focused Frontend Developer with 5 years of commercial experience building
business web applications: CRM-style systems, analytics dashboards, admin panels and
internal tools. Strong in Angular, TypeScript, RxJS, REST API integration, reusable UI
components, data-heavy tables, forms and charts, and performance work on interfaces
that render thousands of rows.

I am comfortable clarifying requirements with stakeholders, implementing UI features
end to end, integrating backend APIs, fixing bugs, reviewing code and keeping the
frontend codebase maintainable. Before moving into software engineering I spent a
decade in financial analytics, which is why I enjoy products where data has to be
turned into something people can actually read.

I joined The Rolling Scopes School Fullstack Engineering course to go back to the
fundamentals — semantic HTML, modern CSS, vanilla JavaScript — and to extend my
backend skills (Node.js, NestJS, PostgreSQL) to a level where I can own a feature
across the whole stack, not only its UI.

---

## Skills

- **Frontend:** Angular (11–21), TypeScript, JavaScript (ES6+), RxJS, Signals, NgRx,
  Nx; React / Next.js fundamentals
- **UI & data:** Angular Material, PrimeNG, Highcharts, ApexCharts, Gridster, HTML5,
  CSS3, SCSS, Tailwind, Bootstrap
- **Web integration:** REST APIs, WebSockets, authentication, tracking and event
  instrumentation
- **Testing:** unit testing, Jest, Jasmine / Karma, Cypress fundamentals
- **Tooling / DevOps:** Git, GitHub, CI/CD (GitLab, Jenkins), Docker, AWS fundamentals
- **Backend:** Node.js, NestJS, Express, PostgreSQL, Prisma ORM, MongoDB, REST API
  development
- **Developer tools:** VS Code, Chrome DevTools, Figma, OpenAI Codex, Claude Code,
  GitHub Copilot

---

## Code Example

RxJS text field input autocomplete with 300ms debounce and switchMap to cancel outdated API requests.

```
readonly search = new FormControl('', { nonNullable: true });

readonly results$ = this.search.valueChanges.pipe(
  map(value => value.trim()),
  debounceTime(300),
  distinctUntilChanged(),
  filter(value => value.length >= 2),
  switchMap(query =>
    this.api.search(query).pipe(
      catchError(() => of([]))
    )
  )
);
```

---

## Experience

### Frontend Engineer (Angular) — Max Momentum LLC

*Remote, US-based company · Jul 2023 — present*

- Developed and maintained Angular applications, analytics dashboards, CRM-style
  workflows and internal monitoring tools for data-heavy business operations.
- Implemented reusable Angular modules, components, services and typed API models
  using TypeScript, RxJS, Signals, Angular Material and PrimeNG.
- Delivered KPI dashboards for campaign performance, revenue, user activity and
  operational metrics, so non-technical teams can monitor the business without
  manual reporting.
- Built data-heavy admin tables with filtering, sorting, pagination, saved column
  settings, loading states and optimised rendering for 1,000+ row datasets.
- Integrated REST APIs with authentication, interceptors, typed models, error
  handling and data refresh flows.
- Created a monitoring system with an admin panel for hundreds of landing pages
  (Node.js / Express, Telegram bot on grammY), reducing manual checks.
- Built a lead management API with NestJS, Prisma and PostgreSQL, and supported an
  existing MongoDB database.

### Frontend Developer — Andersen Lab

*Remote, Poland · Jan 2021 — Jul 2023*

- Worked on commercial Angular projects in Healthcare and FinTech domains: CRM
  modules, dashboards, scheduling workflows and API-driven business features.
- TaskDent Healthcare CRM: developed Angular 15 modules with NgRx, forms, tables,
  dashboards and REST API integration.
- Built interactive financial, patient-activity and operational dashboards with
  ApexCharts.
- Internal scheduling tool: real-time room reservation system on Angular 11 and
  WebSockets.
- Improved code quality through code reviews, refactoring, regression fixes and unit
  tests with Jasmine / Karma; worked in Agile / Scrum teams with backend, QA and
  business stakeholders.

### Data Analyst, Financial Analysis Department — Belgazprombank

*Belarus · Jan 2010 — Jan 2021*

- Automated financial reporting and analytical workflows with Power BI, SQL, Python
  and VBA / Excel.
- Built dashboards and reporting tools, then transitioned into software engineering
  and frontend development.

---

## Education

- **The Rolling Scopes School** — Fullstack Engineering course, 2026 — present.
  Frontend and backend fundamentals, code review and cross-check practice.
- **Belarus State Economic University** — BSc in Economic Cybernetics

---

## Languages

- **English — B2+.** Daily working language for the last five years: stand-ups and
  planning with a US-based team, technical documentation, code reviews and Pull
  Request discussions in English.
- **Polish — basic.**
- **Russian, Belarusian — native.**