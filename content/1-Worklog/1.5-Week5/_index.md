---
title: "Week 5 Worklog"
date: 2026-10-16
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Join the FCAJ Hackathon System team and agree on the problem, target users and goals of the workshop.
* Get access to the team repository and understand how the existing SEAL Hackathon system is organized.
* Take part in renaming the project from SEAL to FCAJ (Issue #1).
* Understand the current frontend stack and how it is built and deployed today.
* Study the Shared Responsibility Model, IAM roles and cost optimization to prepare for the AWS design.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Team brainstorming: problem, users (organizers, participants, judges) and goals of the workshop <br> - Studied the Shared Responsibility Model | 10/12/2026 | 10/12/2026 | [Shared Responsibility Model](https://www.youtube.com/watch?v=tsobAlSg19g); [AWS Well-Architected](https://docs.aws.amazon.com/wellarchitected/latest/framework/the-pillars-of-the-framework.html) |
| 3 | - The team lead created the project repository from the SEAL source code; I cloned it and reviewed the structure: `back-end/seal-api` (Spring Boot), `front-end/seal-web`, `docker-compose.yml`, `Caddyfile`, `docs/` <br> - Studied IAM policies and roles | 10/13/2026 | 10/13/2026 | [Initial commit](https://github.com/nhatnhm1405/fcaj-hackathon-system/commit/35479425a228928d66fa4c73528955925f44f725); [IAM](https://www.youtube.com/watch?v=N_vlJGAqZxo), [Create IAM Role](https://www.youtube.com/watch?v=pJWANviu8QM) |
| 4 | - Assigned to [Issue #1 – Rename files, packages](https://github.com/nhatnhm1405/fcaj-hackathon-system/issues/1) (SEAL → FCAJ) together with the lead and Backend 2 <br> - Listed the frontend parts affected by the rename (folder `seal-web`, app name, texts) | 10/14/2026 | 10/14/2026 | [Issue #1](https://github.com/nhatnhm1405/fcaj-hackathon-system/issues/1); [Refactor commit](https://github.com/nhatnhm1405/fcaj-hackathon-system/commit/3c0de1e3ee9f053c43bf58a355164f0e1ad039c2) |
| 5 | - Reviewed the frontend stack: React 18 + TypeScript + Vite 6, Tailwind CSS 4, MUI / Radix UI, React Router, tests with Vitest and Playwright <br> - Learned how the API address is passed at build time (`VITE_API_URL` build argument) and how the build is served by Caddy in Docker <br> - Studied cost optimization | 10/15/2026 | 10/15/2026 | [Project repository](https://github.com/nhatnhm1405/fcaj-hackathon-system); [Vite env variables](https://vite.dev/guide/env-and-mode); [Cost Optimization](https://www.youtube.com/watch?v=IY61YlmXQe8) |
| 6 | - Reviewed the current deployment: Docker Compose (MySQL, backend, frontend, Caddy) and the GitHub Actions workflow that runs Vitest + JUnit and deploys to EC2 over SSH <br> - Noted what the frontend needs when moving to AWS: static hosting, HTTPS, API URL per environment | 10/16/2026 | 10/16/2026 | [docker-compose.yml](https://github.com/nhatnhm1405/fcaj-hackathon-system/blob/main/docker-compose.yml); [deploy.yml](https://github.com/nhatnhm1405/fcaj-hackathon-system/blob/main/.github/workflows/deploy.yml) |

### Week 5 Achievements:

* Joined the team and agreed on the problem, users and goals of the workshop.
* Understood the structure of the project repository and the role of each part (backend, frontend, Docker Compose, Caddy, docs).
* Took part in Issue #1 (SEAL → FCAJ rename) and identified the frontend parts affected.
* Understood the frontend stack (React + TypeScript + Vite + Tailwind) and that `VITE_API_URL` is fixed at build time, so each environment needs its own build.
* Understood the current pipeline (tests → deploy to EC2 with Docker Compose) as the starting point for the AWS design.
* Strengthened my knowledge of the Shared Responsibility Model, IAM roles and cost optimization.

<!-- [TO CONFIRM: check the meeting dates and remove this line.] -->
