---
title: "Buildrathon Kickoff: Code the Future with CMC Global"
date: 2026-09-26
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

### Event information

- **Date:** September 26, 2026
- **Start time:** 9:00 a.m. (UTC+7)
- **Location:** Bitexco Financial Tower, Ho Chi Minh City
- **Role:** Attendee
- **Event page:** [Buildrathon Kickoff: Code the Future with CMC Global](https://luma.com/8fe9vvps)

### Event objectives

- Introduce the Buildrathon program and what participants are expected to build.
- Show how cloud and AI knowledge is used in real products through an example from industry.
- Let FCAJ interns meet the speakers and ask questions directly.

### Speakers

| Order | Speaker | Position | Contribution to the event |
| --- | --- | --- | --- |
| 1 | [Hung Gia Nguyen](https://www.linkedin.com/in/jotaguy/) | Head of Solutions Architect, AWS Vietnam and Cambodia | Opened the event, introduced Buildrathon and its direction within the First Cloud AI Journey. |
| 2 | [Truong Nhat Bui](https://www.linkedin.com/in/dominicbui0000/) | Tech Lead, CMC Global | Presented the architecture of an AI-enabled Slack bot built at CMC Global and answered questions. |

The event moved from the "why" (the program and its goals) to the "how" (a real system built by an engineering team), which made the second talk easier to follow.

### Key highlights

#### 1. Buildrathon and the First Cloud AI Journey

The opening talk explained what Buildrathon is, why it is part of the internship and what kind of outcome participants should aim for. The slides also showed a timeline of AWS in Vietnam, from the first local customers to the Local Zone, grouped into three directions: local talent, infrastructure and future skills. This helped me see the internship as part of a longer plan to build cloud and AI skills in Vietnam.

#### 2. A real example: the Market Slack Bot

The CMC Global talk walked through a Slack bot that the team built step by step. The main message on the slide was that each component exists because it solved a real problem the team faced.

| Component | What it does |
| --- | --- |
| Slack + Socket Mode (WebSocket) | Receives mentions, direct messages and messages in active threads. |
| Response gate | Decides whether the bot should answer a message before the AI is called. |
| Claude Code | Generates the answer and returns structured output (JSON). |
| `SOUL.md` + Memory | Defines the bot's voice and scope, and keeps the context of each thread. |
| bot-schedule, Internal API, Cron + database | Run planned turns and app-owned jobs, and store memory and scheduled jobs. |

#### 3. Building step by step

The speaker explained that the bot started with a single use case (triage) and grew over time. New parts were added only when a real need appeared, instead of designing everything at the start.

### Key takeaways

- An AI feature is more than a model call: it also needs a way to receive requests, decide when to respond, keep context and run scheduled work.
- Starting small and adding components only when needed keeps a system easier to understand and maintain.
- Seeing AWS's long-term plan in Vietnam gave more meaning to the skills I am learning in the program.

### Applying the learning

Our team project, the FCAJ Hackathon System, also has an AI component that judges submissions in the background. From this talk, I want to keep the same habits for my Frontend part: give each part one clear job, show the user what state their request is in, and only add features when the team actually needs them.

### Event experience

This was the first event I attended during the internship. Listening to an AWS Solutions Architect and a Tech Lead from CMC Global in the same morning helped me connect the purpose of the program with how engineers build real AI products. After the talks, I took a group photo with the speaker and other FCAJ interns.

### Event photos

![The opening presentation introducing the AWS First Cloud AI Journey.](/images/4-EventParticipated/4.1-Event1/opening-presentation.jpg)

*The opening presentation about the First Cloud AI Journey and Buildrathon.*

![A slide showing the history of AWS investment in Vietnam from 2015 to 2026.](/images/4-EventParticipated/4.1-Event1/aws-vietnam-timeline.jpg)

*The timeline of AWS investment in Vietnam: local talent, infrastructure, skills and future talent.*

![The CMC Global Tech Lead presenting the Market Slack Bot architecture.](/images/4-EventParticipated/4.1-Event1/cmc-global-talk.jpg)

*The CMC Global talk about building an AI-enabled Slack bot.*

![A close-up of the Market Slack Bot architecture slide.](/images/4-EventParticipated/4.1-Event1/slack-bot-architecture.jpg)

*The full architecture of the Market Slack Bot.*

![Group photo with the speaker and FCAJ interns at the Buildrathon Kickoff.](/images/4-EventParticipated/4.1-Event1/buildrathon-kickoff.jpg)

*Group photo with the speaker and FCAJ interns after the event.*
