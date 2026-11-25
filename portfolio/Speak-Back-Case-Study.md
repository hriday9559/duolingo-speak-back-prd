# SPEAK BACK

## Turning daily language-learning habits into real conversations

**Product Management Case Study**  
Independent student project · 2026

**Author:** Hriday Patel  
**Focus:** Product strategy · User research · Prioritisation · Prototyping  
**Stage:** Concept and early prototype validation

---

## The idea

Speak Back is a proposed Duolingo feature that lets learners exchange short, prompted voice messages with mutual friends. It aims to make real-person speaking practice structured, flexible and low-pressure.

## The product question

> How might we help learners move from practising a language inside an app to using it with another person, without needing to schedule a live call?

*Independent portfolio concept. Not affiliated with, endorsed by, or produced by Duolingo.*

**At a glance:** 53 cleaned survey responses · 6 interviews · 5-product desk review · 6-screen Figma prototype · 3 prototype testers

---

# 01 | Discover the problem

I investigated a possible gap: learners may build a consistent learning habit without feeling confident holding a real conversation. Survey and interview research helped assess the problem and preferred practice formats.

### Survey snapshot

| Measure | Result |
|---|---:|
| Cleaned survey responses | **53** |
| Rated conversation ability 1–2 out of 5 | **30 / 53** |
| Said they would like peer practice | **25 / 51** |

### Self-rated speaking ability (N=53)

| Rating | Responses |
|---|---:|
| 1 · Very low | 11 |
| 2 | 19 |
| 3 | 17 |
| 4 | 6 |
| 5 · High | 0 |

**Mean self-rating: 2.34 / 5.** No respondent selected 5.

### Preferred practice format (N=51)

| Format | Responses |
|---|---:|
| Voice message · friend | 17 |
| Live · friend | 12 |
| Voice message · stranger | 6 |
| Live · stranger | 3 |
| None | 13 |

29/51 selected a friend-based format; 23/51 selected a voice-message format. These categories overlap and reflect stated preference, not actual usage.

### Six user interviews

Six approximately 15-minute interviews were conducted in November 2026: three active and three lapsed Duolingo learners. All six described some difficulty using what they had learned in real conversations. Notes—not verbatim transcripts—also showed a preference for lower-pressure asynchronous practice, mixed preferences for friends versus matched learners, and interest in re-recording.

### Research limitations

Two Google Forms were merged; 55 responses were received and 53 retained after cleaning. Respondents came primarily from the author's network. The sample is directional, not representative of Duolingo's user base.

---

# 02 | Competitive context and product choice

Desk research suggests the component behaviours already exist elsewhere. The opportunity is not to claim a new format, but to test whether a particular combination fits Duolingo's learning and social context.

### Competitive context

| Product | Observed speaking / social approach | Implication for Speak Back |
|---|---|---|
| **Duolingo** | Speaking exercises and AI-led conversation experiences. | Peer exchange could complement—not replace—existing practice. |
| **HelloTalk** | Voice messages, calls, translation and language-community tools. | Voice messaging itself is not unique; safety and community design matter. |
| **Tandem** | Language partners with text, voice notes and calls. | Partner discovery is a more complex alternative to friends-first. |
| **Speak** | Structured AI speaking practice and feedback. | AI can support practice, but does not create a human exchange. |
| **Babbel** | Scenario-based AI speaking practice in its Speak experience. | Scenario structure and guided practice are established patterns. |

*Method note: competitor observations are based on public product and help materials, not hands-on testing. Features, pricing and availability may vary by market, plan and release.*

### The product choice

I compared three directions and selected asynchronous voice messages between mutual friends as the smallest testable first release.

| Direction | Why it was considered | Why it was / wasn't selected |
|---|---|---|
| **A · Friend voice messages** | Low scheduling burden; builds on existing relationships. | **Selected:** focused first test, while acknowledging friend availability risk. |
| **B · Matched live calls** | Richer real-time conversation. | **Deferred:** matching, scheduling and safety add complexity. |
| **C · Group speaking rooms** | Shared social practice. | **Deferred:** moderation and coordination make it a larger first bet. |

### Differentiation hypothesis

Course context + existing social relationships + short asynchronous human exchanges + integration into an established learning habit may create a useful combination. This remains a hypothesis to validate.

---

# 03 | Define and prioritise the MVP

**Problem statement:** Learners building a daily language-learning habit may still lack a low-pressure way to speak with a real person, limiting opportunities to practise conversational confidence.

**Product vision:** Make real-person speaking practice a natural extension of the language-learning habit.

### MVP scope

| In scope · MVP | Out of scope · first release |
|---|---|
| Voice messages up to 60 seconds | Live calls |
| Eligible mutual friends only | Stranger matching |
| Course-level prompts | Public voice rooms |
| Helpful phrases / examples | AI speaking feedback |
| Playback and re-recording | Direct monetisation |
| Two-way conversation thread | Tutors or teachers |
| Report, block and mute controls | Mandatory contribution to daily lesson streak |
| Separate speaking activity indicator | |

### Prioritisation logic

The original RICE comparison favoured the friend-based asynchronous concept. Scores below are directional because reach, impact and confidence were estimates—not measured product data.

| Concept | Reach | Impact | Confidence | Effort | RICE |
|---|---:|---:|---:|---:|---:|
| Friend voice messages | 6 | 2 | 60% | 4 | **1.80** |
| Stranger live calls | 8 | 3 | 30% | 10 | **0.72** |
| Live group rooms | 3 | 2 | 20% | 8 | **0.15** |

RICE = Reach × Impact × Confidence ÷ Effort. Treat these scores as a prioritisation aid, not proof that the selected option will perform best.

### Key trade-offs

**Friend availability:** Users without eligible friends may not reach the core experience. Provide a clear empty state; do not silently route them into stranger matching.

**Reply latency:** Asynchronous exchanges may remain incomplete. Measure first-message reply rate and time-to-reply before adding nudges.

**Habit integration:** Keep speaking activity separate from the daily lesson streak initially; do not make peer participation mandatory to preserve an existing habit.

**Safety:** Mutual-friend access does not remove risk. Reporting, blocking, moderation, age requirements and privacy controls need product, policy and legal review.

**Behavioural segments:** Hesitant speaker, time-constrained learner and socially cautious / independent learner. These are research-informed behaviour patterns, not demographic personas.

---

# 04 | Prototype walkthrough

The six-screen Figma prototype visualises the proposed end-to-end flow. These are individual screens from the design file.

## 01 · Home

Entry point: Speak Back appears in the learning path alongside the regular lesson.

## 02 · Choose friend

Friends-only selection makes the first-release boundary explicit.

**Flow:** Home → Choose friend → Prompt → Record & review → Conversation → Safety controls.

## 03 · Speaking prompt

A course-relevant topic and phrase hints help learners get started.

## 04 · Record & review

Learners can listen back, re-record and send a message up to 60 seconds.

**Design intent:** Lower pressure through structure, short duration, helpful language and the ability to review before sending.

## 05 · Conversation

The thread shows both sides of the exchange and marks the exchange as completed.

## 06 · Safety

Learners can report, block, mute notifications or remove speaking access.

**Prototype disclosure:** Audio is simulated in this interactive student prototype. Names and avatars are fictional.

---

# 05 | Define success and test the hypothesis

The proposed North Star Metric is **Weekly Speaking Learners (WSL):** unique eligible learners who complete at least one two-way speaking exchange in a calendar week. All targets below are hypotheses, not observed results.

### Metrics

| Metric | Proposed target / definition | Interpretation |
|---|---|---|
| **WSL** | Unique learners with at least one two-way exchange per week. | Core completed behaviour. |
| **8-week adoption** | 5% of eligible users complete at least one two-way exchange by week 8. | Cumulative early adoption target. |
| **First-send rate** | 15% of eligible users send at least one first message during the measurement window. | Tests whether users start. |
| **24-hour reply rate** | 40% of first messages receive a reply within 24 hours. | Tests whether exchanges become two-way. |
| **Repeat frequency** | 2+ completed exchanges per active speaking learner per week. | Tests repeat behaviour. |

### Experiment proposal

Run a 50/50 cluster-randomised experiment among eligible adult mobile users in a small set of languages. Randomise friend clusters to reduce treatment/control spillover. Run for at least four weeks; calculate sample size from the actual baseline and account for clustering before launch.

### Guardrails

Monitor daily lesson completion, streak breaks, reports per 1,000 speaking learners, blocks / mutes and user feedback. A rise in speaking activity is not a success if it harms core lesson behaviour or creates unacceptable safety risk.

### What this project has not established

The survey, interviews and prototype do not prove improved retention, learning outcomes or product-market fit. Those are outcomes to test in a properly designed live experiment—not claims to make from this project.

**Measurement note:** Define eligibility, exposure, event instrumentation, deduplication and the experiment's primary outcome before launch. The proposed adoption and send-rate targets use different event definitions and should not be treated as interchangeable.

---

# 06 | Prototype feedback and next steps

The interactive prototype was reviewed with three participants. All three found the core experience understandable, and no major problems were reported. Treat this as an informal, early usability signal—not evidence of usability at scale or product-market fit.

### Feedback and response

**Optional AI feedback on a specific voice message:** Participants suggested AI analysis to help learners understand where they could improve. Keep this outside the MVP. Any future test should require explicit per-message permission, be off by default, and keep feedback private to the sender. Validate demand, quality, privacy, feasibility and cost first.

**Safety concerns:** Some participants raised safety questions. Existing PRD safeguards were discussed, but this small test did not prove that risks were resolved.

**Recording:** Audio capture was simulated. Real microphone permissions, upload, playback reliability, moderation and abuse handling remain untested.

### Roadmap

| Release | Scope | Gate to progress |
|---|---|---|
| **MVP** | Async voice messages, mutual friends, prompts, phrase hints, replay / re-record, thread and safety controls. | Validate first-send, reply and safety signals. |
| **Next** | Notifications, speaking history, reactions, transcripts and invite links. | Prioritise only after observing core behaviour. |
| **Explore later** | Opt-in partner matching, per-message AI feedback, live calls and social quests. | Require evidence of demand and feasibility. |

### Next validation steps

1. Test with a broader and more diverse set of learners.
2. Validate friend availability and willingness to send a first voice message.
3. Test real audio capture, moderation and safety workflows before any live pilot.
4. Revisit scope after observing actual two-way exchange behaviour.

---

# 07 | Reflection

The biggest product lesson from this project was that a promising feature idea is not enough. The work is deciding which user problem to solve first, what evidence supports the direction, what to leave out, and how to measure whether the experience changes behaviour.

### What this project demonstrates

- Problem framing from directional research
- Combining survey signals with qualitative interviews
- Desk-based competitor analysis
- MVP definition and assumption-led prioritisation
- Product trade-offs across usability, safety and habit design
- Prototype design and early usability feedback
- Metric definition and experiment planning

### Limitations and honesty

This is an independent concept project. It has not been built, launched or tested with Duolingo users. The survey sample is small and network-based; interview notes are summaries, not verbatim transcripts; competitor research was desk-based; prototype audio was simulated; and the three-person usability check is too small to establish usability at scale. Proposed metrics and experiment results do not exist yet.

### Project materials

- **Main product requirements document:** [Speak Back PRD v0.4](../docs/Speak-Back-PRD-v0.4.md)
- **GitHub · PRD and research repository:** https://github.com/hriday9559/duolingo-speak-back-prd
- **Figma · Interactive prototype:** https://www.figma.com/design/PjPuEXfLOmN1UfnXrM6uVc/Duolingo---Speak-Back-Prototype-v1?node-id=0-1

---

## SPEAK BACK

### Learn it. Say it. Share it.

Hriday Patel · Independent student project · 2026
