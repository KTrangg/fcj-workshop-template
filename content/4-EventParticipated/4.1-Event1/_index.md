---
title: "Event 1"
date: 2026-09-26
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# Summary Report: “Buildrathon Kickoff: Code the Future with CMC Global”

### Event Information

- **Date & Time:** 09:00, September 26, 2026
- **Location:** Bitexco Financial Tower, Ho Chi Minh City
- **Role:** Attendee
- **Event page:** [Buildrathon Kickoff: Code the Future with CMC Global](https://luma.com/8fe9vvps)

### Event Objectives

- Introduce the Buildrathon program, its goals and what participants are expected to build.
- Connect cloud and AI learning with real examples from industry engineers.
- Give FCAJ interns a chance to talk directly with the speakers.

### Speakers

- **Nguyen Gia Hung** – Head of Solutions Architect, AWS Vietnam and Cambodia
- **Bui Truong Nhat** – Tech Lead, CMC Global

### Key Highlights

#### Buildrathon program introduction

- The opening session explained the purpose of Buildrathon and how it fits into the First Cloud AI Journey.
- The slides gave context on AWS in Vietnam: investment in local talent, infrastructure and future skills.

#### Example architecture: an AI-enabled Slack bot

The technical talk walked through a Slack bot architecture made of several connected parts:

- **Slack + Socket Mode (WebSocket):** receives mentions, direct messages and thread replies.
- **Response gate:** decides whether and when the bot should answer before calling the AI.
- **AI processing (Claude Code):** produces the answer as structured output.
- **Configuration and memory:** a file that defines the bot's voice and scope, plus thread context.
- **Scheduler, internal API and database:** run planned tasks and store data for memory and jobs.

### Key Takeaways

- An AI application is more than a model call: it also needs request handling, response control, context and scheduled work.
- Splitting a system into clear components makes it easier to explain, test and extend.
- Events like this help connect what I study in the FCJ modules with how engineers build real products.

### Applying to Work

- Our FCAJ Hackathon System also has an AI component (the AI judge worker). The idea of a "gate" before the AI and a clear job flow is useful when designing how the frontend shows each job state.
- When drawing our architecture, I will separate request handling, processing and storage the same way the speaker did.

### Event Experience

This was my first event during the internship. Listening to an AWS Solutions Architect and a Tech Lead from CMC Global helped me understand what Buildrathon expects and how an AI feature is put together in a real system. It was also a good chance to meet the speakers and other interns in person.

#### Event photo

![Group photo with the speaker and FCAJ interns at the Buildrathon Kickoff](/images/4-EventParticipated/4.1-Event1/buildrathon-kickoff.jpg)

*Group photo with the speaker and FCAJ interns at the Buildrathon Kickoff, Bitexco Financial Tower.*
