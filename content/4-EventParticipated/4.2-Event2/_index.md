---
title: "AWS Cloud and AI Day Hanoi 2026: HCMC Watch Party"
date: 2026-09-29
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

### Event information

| Item | Details |
| --- | --- |
| **Event** | AWS Cloud and AI Day Hanoi 2026 |
| **Date** | September 29, 2026 |
| **Time** | 8:00 a.m. to 5:00 p.m. (UTC+7) |
| **Format** | Watch party in Ho Chi Minh City, following the program streamed live from Hanoi |
| **Watch party venue** | 26th floor, Bitexco Financial Tower, 2 Hai Trieu Street, Saigon Ward, Ho Chi Minh City |
| **My role** | Attendee |
| **Event links** | [AWS Cloud and AI Day Hanoi](https://aws.amazon.com/events/cloud-day-hanoi/) · [Watch party information](https://apj.awsevents.com/sites/aws-cloud-day-hanoi-watch-party-attendee) |

On September 29, 2026, I joined the Ho Chi Minh City watch party of AWS Cloud and AI Day Hanoi together with other FCAJ interns. We followed the keynote streamed from Hanoi, which covered how cloud and AI are used in Vietnam, the engineering behind reliable cloud services, and how to keep software quality when AI speeds up development.

### Event objectives

- Learn how organizations in Vietnam use cloud and AI in their daily work.
- Understand the infrastructure, security and governance needed to run AI beyond experiments.
- See why AI-assisted development still needs testing, evidence and human review.
- Find cloud and AI topics I can apply to the team project.

### Keynote speakers

| Order | Speaker | Title | Main topic |
| --- | --- | --- | --- |
| 1 | Hoang Minh | Deputy Minister of Science and Technology | Digital infrastructure, compute capacity and Vietnam's cloud and AI ecosystem. |
| 2 | Jennifer Wicks | U.S. Ambassador to Vietnam | Technology cooperation and the role of cloud in digital transformation. |
| 3 | Eric Yeo | Country General Manager Malaysia, Vietnam, Indochina, AWS | Customer examples, infrastructure and skills development in Vietnam. |
| 4 | Dr. Jens Lottner | Chief Executive Officer, Techcombank | Bringing AI into enterprise workflows and training staff. |
| 5 | Dr. Werner Vogels | Chief Technology Officer, Amazon.com | The engineering behind cloud services and system design decisions. |
| 6 | Mai Le | Director of Product Management, Katalon | Validating software quality as AI speeds up development. |

### Key highlights

#### 1. Vietnam's cloud and AI ecosystem

The opening speeches focused on what is needed to create value from AI: digital infrastructure, compute capacity, skilled people and cooperation between government, businesses and universities. The U.S. Ambassador also talked about cloud as a driver of innovation and technology cooperation between the two countries.

#### 2. Starting from customer problems

Eric Yeo shared customer examples in healthcare, retail and agriculture. What I noticed is that each example started from a concrete problem, then chose data and cloud services to solve it. He also mentioned the AWS Local Zone in Hanoi as a way to run workloads closer to users in Vietnam.

#### 3. Techcombank: AI inside the workflow

Dr. Jens Lottner presented AI as a way to change how work is done, not just an extra tool. Examples included linking requirements, development and testing, and helping staff prepare information when handling customer issues. He also stressed access control, choosing the right model, training people and measuring results.

#### 4. Werner Vogels: the engineering users do not see

Dr. Werner Vogels explained that good architecture starts from real requirements and from how the application accesses its data. He used examples such as the AWS Nitro System, Lambda with Firecracker and Lambda SnapStart to show the hidden work behind performance, isolation and reliability. He also talked about time in distributed systems and why timestamps need to carry uncertainty.

#### 5. Katalon: testing has to keep up

Mai Le described the gap that appears when code is produced faster than it can be tested. An AI agent needs context from requirements, code changes, test cases and production data to decide what to test. A confident answer from AI is not proof that the software works; teams still need test results, logs and screenshots.

#### 6. Validation debt and accountability

In the closing part, Werner Vogels came back to "validation debt": the unverified work that builds up when changes ship faster than they are checked. The message was clear: speed is useful only if testing and responsibility keep up with it.

### Key takeaways

- **Start with the problem:** define users, workflow and the expected result before picking a model or service.
- **Design for control:** AI components need limited permissions, defined tools and activity that can be observed.
- **Prove it with evidence:** tests, logs and metrics show what really happened.
- **Understand the trade-offs:** performance, isolation, cost and reliability all shape a design.
- **People stay responsible:** AI can help build and test, but engineers decide whether to release.

### Applying the learning

In the FCAJ Hackathon System, an AI worker scores submissions in the background. For my Frontend part, this means the UI must show clearly whether a job is waiting, processing, done or failed, and the team should keep logs so every AI result can be checked later. When I test the frontend, I will keep test results and screenshots as evidence.

### Event experience

Watching the keynote with other FCAJ interns in Ho Chi Minh City let me follow a large AWS event without going to Hanoi. The talks mixed business and engineering views, which helped me see how the cloud foundations I studied in the first weeks (networking, compute, storage) support real AI products.

### Watch party photos

![The Ho Chi Minh City watch party room with FCAJ interns following the keynote streamed from Hanoi.](/images/4-EventParticipated/4.2-Event2/cloud-ai-day-watch-party.jpg)

*The watch party room on the 26th floor of Bitexco Financial Tower during the keynote.*

![Attendees at the watch party with the feedback form shown on the screens.](/images/4-EventParticipated/4.2-Event2/watch-party-closing.jpg)

*The end of the session, with the event feedback form shown on the screens.*

### References

- [AWS Cloud and AI Day Hanoi: event and speaker information](https://aws.amazon.com/events/cloud-day-hanoi/)
- [AWS Cloud Day Hanoi: Ho Chi Minh City watch party](https://apj.awsevents.com/sites/aws-cloud-day-hanoi-watch-party-attendee)
- [AWS Lambda SnapStart](https://docs.aws.amazon.com/lambda/latest/dg/snapstart.html)
