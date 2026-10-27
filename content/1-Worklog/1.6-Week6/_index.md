---
title: "Week 6 Worklog"
date: 2026-10-23
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:

* Follow the project's survey and proposal phase (project week 1) from the Frontend side.
* Choose a way to host the frontend on AWS and understand what it needs (HTTPS, caching, SPA routing, API URL).
* Check that the frontend still builds and passes tests after the SEAL → FCAJ rename.
* Understand the target AI judging flow so the UI can show each job state.
* Prepare inputs for the frontend part of the proposal (architecture, cost).

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - The project was renamed to FCAJ Hackathon (README updated) <br> - Compared frontend hosting options on AWS: keep the container on EC2 (current), S3 + CloudFront, AWS Amplify Hosting | 10/19/2026 | 10/19/2026 | [Rename commit](https://github.com/nhatnhm1405/fcaj-hackathon-system/commit/087fb7e9372c8d07b167772c764f96e4b0d51a11); [Amplify Hosting](https://docs.aws.amazon.com/amplify/latest/userguide/welcome.html); [Hosting a static website on S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html) |
| 3 | - Researched S3 + CloudFront for a single-page app: private bucket with Origin Access Control, custom error response returning `index.html`, cache invalidation after each deploy <br> - Noted that `VITE_API_URL` must be set in the CI build because it is bundled at build time | 10/20/2026 | 10/20/2026 | [Restrict access to an S3 origin (OAC)](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html); [Custom error responses](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/GeneratingCustomErrorResponses.html); [Invalidating files](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Invalidation.html) |
| 4 | - PR #10 (`feature/technical-rename-fcaj`) was merged into `main` <br> - Pulled the latest `main` and checked the frontend locally: `npm ci`, `npm run build`, `npm test` (Vitest) | 10/21/2026 | 10/21/2026 | [Merge commit PR #10](https://github.com/nhatnhm1405/fcaj-hackathon-system/commit/93c3cbab5b7e42cc4a19e2e7b6eeaf45913d91b4); [Vitest](https://vitest.dev/guide/) |
| 5 | - Studied the target flow: Frontend → Backend → RDS/S3 → AI job → SQS → worker → result → Backend → Frontend <br> - Listed the job states the UI must show (waiting, processing, succeeded, failed) and the API data the frontend needs from Backend 1 | 10/22/2026 | 10/22/2026 | [Amazon SQS](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html); [Project repository](https://github.com/nhatnhm1405/fcaj-hackathon-system) |
| 6 | - Prepared cost inputs for the frontend (S3 storage, CloudFront requests and data transfer) for the proposal estimate <br> - Summarized the frontend proposal: hosting choice, CORS and login cookie points to check with the backend | 10/23/2026 | 10/23/2026 | [AWS Pricing Calculator](https://calculator.aws/); [CloudFront pricing](https://aws.amazon.com/cloudfront/pricing/) |

### Week 6 Achievements:

* Chose S3 + CloudFront as the target hosting for the frontend and understood its requirements: private bucket with OAC, SPA fallback to `index.html`, cache invalidation.
* Understood that the API URL is bundled at build time, so the CI pipeline must build the frontend with the correct `VITE_API_URL` for each environment.
* Confirmed the frontend builds and passes its tests after the rename merged in PR #10.
* Understood the AI job flow through SQS and listed the UI states and API data needed.
* Prepared the frontend inputs for the proposal and the cost estimate, ready for the Week 2 task in [Issue #12](https://github.com/nhatnhm1405/fcaj-hackathon-system/issues/12).

<!-- [TO CONFIRM: check day 4 (did you run build/test locally?) and add links to your notes or proposal section, then remove this line.] -->
