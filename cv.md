---
title: Aliaksandr Dvaraninau — CV
description: Frontend Developer — Angular / TypeScript
---

# Aliaksandr Dvaraninau

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