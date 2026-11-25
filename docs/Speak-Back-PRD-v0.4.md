# Speak Back — Product Requirements Document

**Version:** 0.4  
**Date:** 25 November 2026  
**Author:** Hriday Patel  
**Status:** Current consolidated PRD  
**Project type:** Independent product-management portfolio project

> Speak Back is an independent product concept. It is not affiliated with, endorsed by, or produced by Duolingo. This document describes a proposed feature, not a product built or approved by Duolingo.

## Document status and change history

This is the **main PRD and current source of truth** for the Speak Back project. It consolidates the original v0.3 requirements with completed survey and interview research, prototype decisions, and the latest UAT findings.

- **v0.4 — 25 November 2026:** Consolidated the full PRD; incorporated completed research, six-screen prototype feedback, UAT results, clarified MVP priorities, and documented known prototype gaps.
- **v0.3 — 19 November 2026:** Original full PRD draft. Preserved in the [archive](archive/Speak-Back-PRD-v0.3.md) for historical reference.

## 1. Executive summary

Speak Back is a proposed Duolingo feature that lets learners exchange short, prompted voice messages with mutual friends. It aims to give learners a low-pressure way to practise speaking with a real person, without requiring a live call or a conversation with a stranger.

The product hypothesis is that combining course-level prompts, helpful phrases, asynchronous voice messages and existing social relationships can help learners move from practising inside the app to using a language with another person.

The selected direction is **asynchronous voice messages between mutual friends**. The initial experience is deliberately narrow: choose a friend, respond to a guided prompt, review and send a short recording, then listen and reply in the same conversation.

Research suggests a potential problem and some interest in peer practice, but the evidence is directional. Six interviews and a three-person prototype walkthrough add qualitative context, not proof of demand or impact. The Figma prototype demonstrates the interaction flow; it does not record real microphone audio.

### Product at a glance

| Item | Current direction |
|---|---|
| Primary user | A Duolingo learner who wants low-pressure real-person speaking practice |
| Core behaviour | Send and receive short prompted voice messages with a mutual friend |
| Platform assumption | Duolingo mobile app |
| MVP boundary | Friends-only, asynchronous, prompt-led voice exchange |
| North Star Metric | Weekly Speaking Learners (WSL) completing a two-way exchange |
| Not in MVP | Live calls, stranger matching, public rooms, AI speech scoring |
| Current artefact | Six-screen interactive Figma prototype |
| Validation status | Three-person prototype walkthrough; 10 UAT checks recorded |

## 2. Background and problem

### 2.1 Product context

Duolingo already supports learning habits and social accountability through features such as Friend Streaks, Friends Quests, leaderboards and speaking exercises. Its AI conversation experiences offer practice with an AI character. These experiences serve different purposes from speaking with another learner.

The opportunity explored here is not to replace existing speaking exercises or AI practice. It is to test whether a short, structured exchange with a real friend can complement them.

Public company and product information used in the original research was checked in November 2026. Product availability, plan access and company metrics can change; public figures below are a dated context snapshot, not live product data.

| Public context snapshot | Figure / observation | Source note |
|---|---:|---|
| Q3 2026 daily active users | 64.9M average | Duolingo Q3 2026 shareholder letter |
| Q3 2026 monthly active users | 153.1M average | Duolingo Q3 2026 shareholder letter |
| Paid subscribers at period end | 13.1M | Duolingo Q3 2026 shareholder letter |
| Friend Streak | Launched in 2024 | Duolingo product blog |
| Friends Quests | Shared goals with a mutual friend | Duolingo product blog |
| Video Call | AI-led spoken conversation experience | Duolingo Q3 2026 shareholder letter |

The paid-subscriber count and MAU figure use different time bases. Any ratio between them is an approximation and should not be presented as an official Duolingo metric.

### 2.2 Research evidence

#### Survey

Two Google Forms collected over approximately six months were merged. There were **55 merged responses**, with **53 retained after cleaning**. Respondents came primarily from the author's network, so results are directional and not representative of Duolingo's user base.

| Finding | Result | Denominator |
|---|---:|---:|
| Rated ability to hold a simple two-minute conversation 1 or 2 out of 5 | 30 | 53 |
| Said they would like to practise with another learner | 25 | 51 |
| Preferred a friend format | 29 | 51 |
| Preferred a stranger format | 9 | 51 |
| Selected a voice-message format | 23 | 51 |
| Selected a live-call format | 15 | 51 |
| Used Duolingo for 1+ year and rated speaking ability 1 or 2 | 11 | 21 |

The friend/stranger and voice/live format figures come from the same preference question and should be interpreted as stated preferences, not observed behaviour. The categories may overlap.

Among respondents who had stopped using Duolingo, 5 of 18 selected wanting to practise real conversation as a reason. Among those considering stopping, 3 of 13 selected that reason. These are small subgroup signals, not evidence that a peer-speaking feature would prevent churn.

#### Interviews

Six interviews were conducted in November 2026, approximately 15 minutes each: three with active Duolingo learners and three with lapsed learners. Interview records are notes and summaries, not verbatim transcripts.

Themes recorded in the interview synthesis included:
- Difficulty turning learned material into natural conversation.
- Interest in lower-pressure asynchronous practice rather than scheduling a live call.
- Mixed preferences for practising with friends versus matched learners.
- Value placed on being able to re-record before sending.

All six interviewees described some difficulty using what they had learned in real conversations. These findings are qualitative and should not be treated as population estimates.

#### What the evidence supports — and does not support

The evidence supports investigating a friends-first, asynchronous speaking concept. It does not prove that learners will send voice messages, that the feature will improve speaking ability, or that it will increase retention.

### 2.3 Problem statement

Learners may build a consistent language-learning habit without feeling confident using the language in a real conversation. They may want to practise with another person but find live calls intimidating, difficult to schedule or too high-pressure.

**Problem statement:** Duolingo learners who want to improve conversational confidence may lack a low-pressure, structured way to practise speaking with someone they know, making it difficult to turn in-app learning into real-person conversation.

### 2.4 Product opportunity

Create a lightweight speaking exchange that:
- Uses existing mutual-friend relationships rather than stranger matching.
- Gives both learners a clear, course-level prompt.
- Lets users record asynchronously and review before sending.
- Keeps the exchange in a simple conversation thread.
- Makes safety controls visible and accessible.

## 3. Product vision, goals and non-goals

### Vision

Make real-person speaking practice a natural, low-pressure extension of the language-learning habit.

### Goals

1. Give learners a way to practise speaking with a real person, including free learners.
2. Reduce the effort and social pressure involved in starting a speaking exchange.
3. Encourage repeat two-way speaking practice with an existing friend.
4. Explore whether the behaviour can complement, rather than displace, daily lessons.
5. Give learners clear controls over who can contact them and how they manage interactions.

### Non-goals for the MVP

1. Live voice or video calls between learners.
2. Matching with strangers or public speaking rooms.
3. Replacing Duolingo's AI conversation experiences.
4. Automated speech scoring or pronunciation grades.
5. Tutors, teachers or scheduled classes.
6. Direct monetisation.
7. Making Speak Back activity count as completion of the daily lesson.

## 4. Target users and key needs

The following are behavioural segments informed by the research. They are not demographic personas or claims about all Duolingo learners.

| Segment | Need | Product implication |
|---|---|---|
| Hesitant speaker | Wants help getting started and time to think before speaking | Guided prompts, helpful phrases, example answers, re-recording |
| Time-constrained learner | Wants practice without scheduling a live session | Asynchronous messages and short recordings |
| Socially cautious learner | Prefers a familiar partner and control over contact | Mutual-friend eligibility, clear consent and safety controls |
| Socially motivated learner | Wants a reason to practise with another learner | Conversation thread, completion state and optional reactions later |

### Primary user story

As a language learner, I want to exchange short, guided voice messages with a mutual friend so that I can practise speaking in a flexible and less intimidating way.

## 5. Product hypotheses

| ID | Hypothesis | Evidence / validation approach | Current status |
|---|---|---|---|
| H1 | Some learners maintain a learning habit but still lack confidence in real conversation | Survey self-rating and interviews | Directional support: 30/53 rated conversation ability 1–2; all six interviewees described some difficulty |
| H2 | Some learners are open to practising with another learner | Survey and interviews | Directional support: 25/51 said they would like peer practice |
| H3 | A friend-based format is more acceptable to this audience than stranger matching | Survey preferences and interviews | Directional support: 29/51 selected friend format vs 9/51 stranger format; interview preferences were mixed |
| H4 | Asynchronous voice messages feel easier to start than live calls | Survey and interviews | Directional support: 23/51 selected voice-message formats vs 15/51 live-call formats |
| H5 | Speaking with a friend can improve engagement or retention without harming lesson behaviour | Live, instrumented experiment | Unvalidated; prototype and research do not establish impact |

H1–H4 are directional signals. H5 requires a properly designed live experiment.

## 6. Solution options and prioritisation

### Options considered

| Option | Description | Advantages | Main challenges | Decision |
|---|---|---|---|---|
| A. Async voice with friends | Prompted voice replies between mutual friends | Low scheduling burden; uses existing relationships; easier first test | Friend availability; delayed replies; voice safety | **Selected** |
| B. Live 1:1 calls with matched strangers | Real-time calls with a learner at a similar level | Richer live conversation | Matching, cold start, scheduling, moderation and safety complexity | Deferred |
| C. Live group speaking rooms | Scheduled group rooms with a host | Shared practice and community | Coordination, moderation and attendance burden | Deferred |

### RICE comparison

RICE = (Reach × Impact × Confidence) ÷ Effort. All values are author estimates for relative comparison only; they are not based on Duolingo internal data.

| Option | Reach | Impact | Confidence | Effort (person-months) | RICE |
|---|---:|---:|---:|---:|---:|
| Async voice with friends | 6 | 2 | 60% | 4 | **1.80** |
| Live 1:1 calls with strangers | 8 | 3 | 30% | 10 | **0.72** |
| Live group speaking rooms | 3 | 2 | 20% | 8 | **0.15** |

**Decision:** Option A is the smallest testable direction. A voice message is not a live conversation, but it tests whether learners will speak to each other at all without first solving matching and scheduling.

### Trade-offs accepted

- Learners without an eligible friend may not be able to use the feature initially. Show a clear empty state; do not silently send users into stranger matching.
- Replies may be delayed. Measure reply rate and time-to-reply before adding nudges.
- Friend-based practice may not suit every learner or language pairing.
- Speak Back should not replace the daily lesson or become a requirement for maintaining a streak.
- Friends-only access reduces some discovery risks but does not eliminate harassment or misuse.

## 7. MVP scope and release priorities

### P0 — Required for an MVP pilot

1. Start Speak Back from a clear entry point in the learning experience.
2. Select an eligible mutual friend who is learning the same target language or has a compatible prompt set.
3. Display a prompt appropriate to the learner's course level.
4. Show three helpful phrases and an optional example answer for each prompt.
5. Allow the user to record a voice message up to 60 seconds.
6. Allow the user to listen to the recording before sending and re-record if needed.
7. Enforce a minimum recording duration of five seconds and a maximum of 60 seconds before enabling Send.
8. Send and receive voice messages in a conversation thread.
9. Play received messages at 1× and 0.75× speed.
10. Show the prompt associated with each message.
11. Provide reporting, blocking and muting controls from the conversation/message context.
12. Provide a setting to turn Speak Back off.
13. Restrict access according to applicable regional age requirements, subject to legal and policy review.
14. Screen voice messages before delivery using an appropriate speech-to-text and content-safety process, with human review for reported messages.
15. Show a “spoke today” indicator after both participants have sent a message in the exchange. It must not replace or complete the daily lesson.
16. Instrument the core funnel, exchange and safety events needed to evaluate the feature.

### P1 — Follow-up opportunities, subject to evidence

- Push notification when a friend sends a Speak Back message.
- Preset reactions such as “Nice!”, “I understood you!” and “Say it again?”
- Speaking history, including first and latest recordings.
- Optional transcript to support listening comprehension.
- Invite link to bring an existing friend onto Duolingo.
- User-controlled AI feedback on an individually selected message. This is a post-MVP hypothesis, not a committed launch requirement.

### P2 — Longer-term ideas

- Opt-in matching with learners at a similar level, only after safety and demand are validated.
- Short live calls with friends.
- Speak Back challenges within Friends Quests.
- Group speaking rooms, only if evidence supports the added complexity.

### Explicitly excluded from the MVP

Live calls, stranger matching, public voice rooms, tutors, automatic AI analysis of every message, public speech scores and direct monetisation.

## 8. User journey and core experience

**Core flow:** Home → Choose Friend → Speaking Prompt → Record & Review → Conversation.

Safety controls are an optional branch from the conversation, not a required final step.

### Screen 1 — Home

**Purpose:** Make the feature discoverable within the existing learning experience.

- Show a Speak Back entry card.
- Explain that the user can practise speaking with a friend.
- Start opens friend selection.
- Dismiss hides the card without affecting the daily lesson.

### Screen 2 — Choose Friend

**Purpose:** Let the learner choose a familiar, eligible partner.

- Show eligible mutual friends.
- Show relevant language and course context.
- Make unavailable or incompatible friends visibly unavailable, with a clear explanation.
- Do not offer stranger matching in the MVP.

### Screen 3 — Speaking Prompt

**Purpose:** Reduce the blank-page problem and help the learner begin.

- Show a prompt in the target language, with a translation where appropriate.
- Show three helpful phrases.
- Provide an optional example answer.
- Allow the learner to shuffle to another prompt at a similar level.
- “I'm ready” proceeds to recording.

### Screen 4 — Record & Review

**Purpose:** Give the learner control before sharing their voice.

- Show a clear microphone/recording state and permission handling.
- Display elapsed time and a 60-second maximum.
- Show a playback preview after recording.
- Allow re-recording.
- Disable Send below five seconds and explain why.
- Enable Send only when the recording meets duration and validation rules.
- Confirm successful send and move to the conversation.

### Screen 5 — Conversation

**Purpose:** Make the exchange understandable and encourage a reply.

- Show messages with sender, prompt context and duration.
- Allow playback at 1× and 0.75×.
- Allow a voice reply in the same thread.
- Show pending, sent, failed and received states clearly.
- Show the “spoke today” indicator only after both participants have sent a message.
- Preset reactions are P1 and are not required for the MVP.

### Screen 6 — Safety Controls

**Purpose:** Give learners fast, understandable control.

- Report a message and select a reason.
- Confirm that a report was received without implying that a moderation decision has already been made.
- Block a user with a clear confirmation step.
- Mute Speak Back notifications from a user.
- Turn off Speak Back through settings.
- Explain the effect of each action.

## 9. User stories and acceptance criteria

| ID | User story | Acceptance criteria |
|---|---|---|
| US1 — Start speaking | As a learner, I want to send a short voice reply to a friend using a prompt so that I can practise speaking without pressure. | I can choose an eligible mutual friend; see a level-appropriate prompt; view three helpful phrases and an optional example; record from 5 to 60 seconds; preview, re-record and send; and receive a clear send confirmation. |
| US2 — Reply to a friend | As a learner, I want to hear and answer my friend's voice reply so that we can practise in a back-and-forth exchange. | I can see the prompt my friend answered; play their message at 1× or 0.75×; and send a voice reply in the same thread. Preset reactions are a P1 enhancement, not an MVP acceptance requirement. |
| US3 — Recognise an exchange | As a learner, I want a completed exchange to be recognised so that speaking feels connected to my social habit. | When both participants have sent a message in the exchange, the thread shows “spoke today”. It does not replace the daily lesson or count as lesson completion. |
| US4 — Get help before speaking | As a nervous learner, I want hints before I speak so that I do not freeze. | Every prompt has three helpful phrases and an optional example answer. The user can shuffle to another prompt at a comparable level. |
| US5 — Stay safe and in control | As a learner, I want to report, block, mute and control who can message me so that I can manage uncomfortable interactions. | Only eligible mutual friends can exchange messages; report and block are accessible from the message/conversation; mute and feature-off controls are available; age eligibility is enforced according to approved regional policy. |
| US6 — Review progress | As a learner, I want to revisit my past recordings so that I can hear how I have progressed. | A dated history and first/latest comparison are defined as a P1 follow-up, not an MVP launch dependency. |

## 10. Functional and non-functional requirements

### Functional requirements

- **Eligibility:** The system checks mutual-friend status, language compatibility, account status and regional age eligibility before allowing an exchange.
- **Prompt selection:** Prompts are mapped to course level and target language. Prompt difficulty should be appropriate to both participants.
- **Recording:** The app requests microphone permission, indicates recording state, enforces 5–60 seconds and handles cancellation or permission denial.
- **Review:** Users can play back their own recording before sending and can replace it.
- **Delivery:** Messages have clear sending, sent, failed and received states. A failed upload can be retried without silently duplicating the message.
- **Playback:** Recipients can play and pause messages and switch between 1× and 0.75×.
- **Safety:** Users can report, block, mute and turn off the feature. Blocking must prevent further contact through Speak Back.
- **Moderation:** Voice content is screened before delivery using an approved policy and technology approach. Reports enter a human review workflow.
- **Analytics:** Events capture exposure, prompt selection, recording start, send, delivery, playback, reply, completed exchange, report, block, mute and feature-off actions.

### Non-functional requirements and design principles

- Recording and playback states must be clear and accessible.
- The experience must handle microphone denial, network interruption, upload failure and app backgrounding without losing or sending unintended audio.
- Audio data must be protected in transit and at rest, with access limited to authorised systems and personnel.
- Retention, deletion, consent and regional privacy obligations require legal and privacy review before a live pilot.
- Moderation must account for supported languages and known speech-to-text limitations. Automated screening must not be treated as a complete safety solution.
- The feature must not degrade core lesson completion or existing Friend Streak behaviour.
- Performance, upload limits, retry behaviour, data retention periods and service-level targets must be specified before engineering release.

## 11. Safety, privacy and trust

Voice messages can contain personal information and can be used for harassment. Mutual-friend access is a boundary, not a guarantee of safety.

### Proposed safeguards

- Mutual-friend eligibility only in the MVP.
- Regional age gating, with exact thresholds confirmed by legal and policy teams.
- Clear explanation of who can hear a message before first send.
- Report and block available from message context.
- Mute and feature-off controls.
- Automated screening before delivery, plus human review for reports.
- Clear moderation policy, escalation process and user-facing reporting confirmation.
- Data minimisation, clear retention periods and deletion controls.
- Privacy notice describing audio processing, storage and access.

### Open implementation dependencies

- Confirm legal basis, consent requirements and regional obligations, including India's DPDP framework and GDPR where applicable.
- Confirm supported languages and quality limits for speech-to-text moderation.
- Define audio storage, retention, deletion and access policies.
- Define report response times, escalation, appeals and repeat-offender handling.
- Conduct a dedicated safety review before any external pilot.

No safety control should be described as fully effective until implemented and tested.

## 12. Success metrics and measurement

### North Star Metric

**Weekly Speaking Learners (WSL):** the number of distinct eligible learners who complete at least one two-way speaking exchange in a calendar week.

A completed exchange means the learner sent at least one voice message and received at least one voice message in the same thread during the measurement window. Count unique learners, not messages.

### Input metrics and proposed targets

| Metric | Definition | Proposed target |
|---|---|---:|
| 8-week adoption | Eligible users who complete at least one two-way exchange by week 8 | 5% |
| First-send rate | Eligible users who send at least one first message after seeing the entry point | 15% |
| 24-hour reply rate | First messages that receive a reply within 24 hours | 40% |
| Repeat frequency | Completed exchanges per active speaking learner per week | 2+ |

These are proposed targets to validate, not measured results or commitments.

### Guardrail metrics

| Guardrail | Definition | Proposed guardrail |
|---|---|---|
| Daily lesson completion | Users completing at least one daily lesson / DAU | No statistically significant decline versus control |
| Reports per 1,000 exchanges | Messages reported / messages sent × 1,000 | Initial target below 2; pause and investigate if exceeded |
| Friend Streak breaks / unfollows | Breaks or unfollows among active Friend Streaks | No significant increase versus control |
| Blocks and mutes | Rate of blocks/mutes among speaking users | Monitor for unexpected increases and investigate |
| Delivery and playback failures | Failed sends or playback attempts / attempts | Define reliability threshold before pilot |

Targets and thresholds must be reviewed against baseline data and safety-team guidance before launch.

### Instrumentation requirements

Define event names, properties, user eligibility, exposure, deduplication and attribution before the experiment. At minimum, instrument:
- Feature impression and entry-point tap.
- Friend list view and friend selection.
- Prompt view and shuffle.
- Recording start, recording complete, duration and re-record.
- Send attempt, send success and send failure.
- Message delivery, playback start, playback completion and playback speed.
- Reply sent and completed exchange.
- Report, block, mute and feature-off.

Do not collect or retain more voice data than is necessary for the feature and approved safety operations.

## 13. Experiment plan

### Objective

Test whether access to Speak Back increases meaningful speaking engagement and whether it affects 28-day retention without harming daily lesson behaviour or safety.

### Proposed design

| Item | Plan |
|---|---|
| Population | Eligible mobile users at or above the approved regional age threshold, with at least one eligible mutual friend |
| Languages | Start with 3–5 languages for which prompts and moderation support are ready |
| Plans | Include free and paid users |
| Randomisation | 50/50 by friend cluster to reduce spillover between treatment and control |
| Initial rollout | Begin with approximately 5% of eligible users after internal and safety checks |
| Control | Existing app experience |
| Treatment | Speak Back MVP |
| Primary outcome | 28-day retention |
| Secondary outcomes | WSL, first-send rate, 24-hour reply rate, repeat exchanges and a one-question speaking-confidence check |
| Duration | At least four full weeks, with sufficient follow-up to measure 28-day retention |
| Minimum detectable effect | Proposed +1 percentage point in 28-day retention; validate feasibility before launch |
| Sample size | Calculate from actual baseline retention, 95% confidence and 80% power; adjust for clustering/design effect |

### Validity risks

1. **Network spillover:** Friendships may cross treatment and control clusters. Measure cross-cluster links and exposure.
2. **Novelty effect:** Review behaviour in later weeks separately from initial adoption.
3. **Selection bias:** Users with eligible friends are not representative of all learners.
4. **Seasonality:** Avoid interpreting holiday, exam or New Year spikes as product effects.
5. **Low-quality exchanges:** Define minimum valid message criteria using duration and speech detection, while monitoring false positives and accessibility impacts.
6. **Safety and moderation capacity:** Do not expand if review queues or safety metrics exceed approved limits.

## 14. Prototype and validation status

### Prototype scope

The Figma prototype contains six screens:
1. Home entry point.
2. Choose a friend.
3. Speaking prompt and hints.
4. Record and review.
5. Conversation.
6. Safety controls.

The prototype is an interactive representation of the proposed experience. **Recording and playback are simulated; it does not capture actual microphone audio.** It does not validate audio quality, real upload, playback reliability, moderation, privacy implementation or actual speaking behaviour.

### Three-person prototype walkthrough

Three participants reviewed the six-screen prototype.

- All three found the core experience understandable.
- No major usability problems were reported.
- Some participants raised safety concerns.
- Some suggested optional AI analysis of an individual voice message, with the user choosing which message may be analysed.

This is early qualitative feedback from three participants. It is not representative evidence and does not establish demand, retention impact or product-market fit.

### UAT results

Fifteen checks are now documented against the clickable Figma prototype: **9 Pass, 5 Fail and 1 Not Run**. These are prototype UI checks, not production validation. The results distinguish MVP requirements from P1 enhancements and include traceability to the user stories.

| Test ID | User story / requirement | Result | Finding |
|---|---|---|---|
| UAT-01 | US1 | Pass | Speak Back opened at Choose a Friend |
| UAT-02 | US1 | Pass | Selected eligible friend carried forward |
| UAT-03 | US1, US4 | Pass | Prompt, helpful phrases and example answer were viewable |
| UAT-04 | US1, US4 | Pass | Shuffle displayed a new prompt and allowed the user to continue |
| UAT-05 | US1 | Pass — UI only | Recording and preview UI flow worked; real audio capture and playback were not tested |
| UAT-06 | US1 | **Fail — UI** | The prototype has no timer or duration indicator and does not prevent a recording under five seconds from being sent |
| UAT-07 | US1 | Pass — UI only | Re-record returned to the recording interface; actual audio replacement was not tested |
| UAT-08 | US1 | Pass | Send confirmation appeared and the conversation screen opened |
| UAT-09a | US2 | Pass — UI only | Playback and 1× / 0.75× speed controls worked |
| UAT-09b | US2 — P1 | **Fail — P1, out of MVP scope** | Preset reactions were not available; reactions are not an MVP acceptance requirement |
| UAT-10 | US5 | Pass — UI flow only | Conversation menu showed Report, Block, Mute and Turn Off; each opened its corresponding prototype screen or confirmation |
| UAT-11 | US1 | **Fail — UI** | No empty state is present for a user with no eligible mutual friends |
| UAT-12 | US1 | **Fail — UI** | Recording-cancel control and microphone-permission-denied state are not represented |
| UAT-13 | US1 | **Fail — UI** | The prototype does not demonstrate enforcement of the 60-second recording maximum |
| UAT-14 | US3 | Not Run | Completed-exchange “spoke today” state has not yet been specifically verified |

### User-story traceability

- **US1 — Start and send a prompted voice reply:** UAT-01–08, UAT-11–13.
- **US2 — Hear and reply to a friend's message:** UAT-09a and UAT-09b. UAT-09b is a P1 enhancement, not an MVP acceptance requirement.
- **US3 — Recognise a completed exchange:** UAT-14.
- **US4 — Get help before speaking:** UAT-03 and UAT-04.
- **US5 — Stay safe and in control:** UAT-10.
- **US6 — Review speaking progress:** Not covered by the current six-screen prototype or this UAT set; speaking history remains P1.

### UAT implications and follow-up

- Add a visible recording timer and implement both the five-second minimum and 60-second maximum.
- Add a clear no-eligible-friends empty state.
- Represent and test recording cancellation and microphone permission denial, including recovery paths.
- Verify the completed-exchange “spoke today” state for US3.
- Preset reactions remain P1 and should not block MVP acceptance. UAT-09b is recorded as a scope gap, not an MVP failure.
- Conduct functional audio testing with real microphone capture, playback, upload failure, retry and permission states before claiming the recording experience is validated.
- Test safety workflows beyond navigation, including actual block enforcement, report handling and moderation response.

The prototype UI failures identify gaps between the current Figma artefact and the written requirements. They do not establish that the product concept itself has failed. “Pass (UI only)” does not validate real audio functionality.

## 15. Roadmap and release gates

| Phase | Scope | Gate to progress |
|---|---|---|
| Discovery and prototype | Research, six-screen prototype, early walkthrough and UAT | Core flow understandable; known gaps documented |
| Functional MVP build | Real recording/playback, friend eligibility, prompts, review, thread, safety and analytics | Audio, privacy, moderation and safety checks pass |
| Controlled pilot | Small eligible population and cluster-based experiment | Primary metric and guardrails reviewed; moderation capacity stable |
| Expansion | Gradual rollout to more eligible users/languages | Reliable systems, acceptable safety metrics and positive evidence |
| Later exploration | Reactions, history, transcripts, invite links and optional AI feedback | Prioritise from observed user behaviour and validated demand |

### Dependencies

- Existing friend graph and Friend Streak systems.
- Audio capture, storage, upload and playback.
- Prompt library and language-learning content design.
- Speech-to-text and content-safety coverage for launch languages.
- Trust & Safety operations and human review.
- Privacy, legal and regional age-policy review.
- Notifications and analytics infrastructure.
- Experimentation support for cluster randomisation.

## 16. Risks and mitigations

| Risk | Why it matters | Mitigation / response |
|---|---|---|
| Harassment or inappropriate content | Voice can carry abuse even between known users | Mutual-friend boundary, age controls, reporting, blocking, screening and human review |
| Moderation quality | Speech-to-text may fail across accents, languages or noisy audio | Validate by language; monitor false positives/negatives; provide human escalation |
| Privacy and data protection | Voice recordings are personal data | Consent, minimisation, deletion, limited retention and legal review |
| Cold start | Users may not have eligible friends | Clear empty state; measure eligible reach; no automatic stranger matching |
| Friend mismatch | Friends may study different languages or levels | Show language and course context; only allow compatible prompt pairings |
| Embarrassment | Users may avoid recording or sharing | Helpful phrases, examples, short duration, preview and re-record |
| Reply latency | One-sided exchanges may discourage users | Measure reply rate and time-to-reply before designing nudges |
| Core learning displacement | Users may substitute messages for lessons | Keep Speak Back separate from lesson completion; monitor lesson guardrail |
| Operational cost | Audio storage, speech processing and review can be expensive | Model per-message costs and moderation capacity before rollout |
| Feature complexity | Live calls and stranger matching introduce large new dependencies | Keep outside MVP; revisit only with evidence |

## 17. Open questions

1. What proportion of active friendships are learning the same language, and how much eligible reach does that create?
2. What is the minimum age for voice features in each launch region?
3. What audio retention period is necessary for delivery and moderation, and what deletion controls are required?
4. What are the moderation costs and quality levels by language?
5. How should the feature handle a friend who never replies?
6. Should the “spoke today” badge ever connect to Friend Streak mechanics, or remain a separate indicator?
7. What is the right threshold for expanding beyond the initial languages?
8. Does Speak Back change retention, speaking confidence or lesson completion in a live experiment?
9. Do learners want reactions, transcripts, history or AI feedback enough to justify their added complexity?

## 18. Post-MVP opportunity: user-controlled AI voice feedback

Some prototype participants suggested optional AI feedback on a voice message they had sent. This is a product hypothesis generated from early feedback, not a validated requirement.

### Proposed experience

1. The user opens a voice message they sent.
2. The user selects **Analyse with AI**.
3. The product explains what will be analysed and how the audio will be processed.
4. The user explicitly confirms permission for that individual message.
5. AI returns private feedback, potentially covering pronunciation, grammar and sentence construction.
6. The user decides whether to keep or act on the feedback.

### Consent and privacy principles

- Off by default; no automatic analysis of every conversation.
- Explicit, message-specific permission.
- Explain audio processing and data handling before confirmation.
- Feedback is private by default and is not shared with the conversation partner unless the user chooses to share it.
- Provide clear controls for analysis and audio data consistent with the product's privacy policy.

### Validation required before prioritisation

Validate demand, preferred feedback types, accuracy, usefulness, privacy expectations, technical feasibility and operating costs. Keep this outside the MVP.

## 19. Competitive context

This is desk research based on public product and help materials, not hands-on testing. Features, pricing and availability may vary by market, plan and release.

| Product | Publicly described approach | Relevance to Speak Back |
|---|---|---|
| Duolingo | Habit-building, friend features, speaking exercises and AI conversation experiences | Speak Back would complement existing learning and AI practice with peer exchange |
| HelloTalk | Language community with text, voice messages and calls | Voice messaging is not unique; safety and structure matter |
| Tandem | Language partners with text, voice notes and calls | Partner discovery is a broader alternative to friends-first |
| Speak | AI-led speaking practice and feedback | AI can support practice but does not create a human exchange |
| Babbel | Structured language learning and AI speaking practice | Guided scenarios are an established learning pattern |

The hypothesis is not that no competitor offers voice messages. The potential distinction is the combination of course-level guidance, an existing social relationship, short asynchronous exchanges and integration into an established learning habit.

## 20. Sources and references

The following public sources informed the original product and competitive context. They should be rechecked before using time-sensitive claims in an external presentation.

- **[S1]** Duolingo, Q3 2026 Shareholder Letter (3 November 2026), SEC filing: https://www.sec.gov/Archives/edgar/data/0001562088/000162828026069474/q3fy26duolingo9-30x26share.htm
- **[S2]** Duolingo Blog, “Friend Streak” (5 August 2024): https://blog.duolingo.com/friend-streak/
- **[S3]** Duolingo Blog, “Product lessons from Friend Streak” (September 2024, updated February 2025): https://blog.duolingo.com/product-lessons-friend-streak/
- **[S4]** Duolingo Blog, “Friends Quests” (2022, updated June 2026): https://blog.duolingo.com/friends-quests/
- **[S5]** Third-party article about Duolingo Events retirement (February 2023; not an official Duolingo source): https://rebeccasdaf.substack.com/p/duolingo-events-retired-but-mine
- **[S6]** Babbel, Conversation Practice / Babbel Speak: https://www.babbel.com/babbel-conversation-practice
- **[S7]** TechCrunch, “Babbel adds live classes, games and more” (2 February 2021): https://techcrunch.com/2021/02/02/language-learning-service-babbel-adds-live-classes-games-and-more/
- **[S8]** Languatalk, “Speak App Review” (competitor-authored review; opinion): https://languatalk.com/blog/speak-app-review/
- **[S9]** TalkDrill, “HelloTalk vs Tandem” (competitor-authored comparison; user counts are self-reported): https://www.talkdrill.com/blog/compare/hellotalk-vs-tandem/

## 21. Related project artefacts

- [Research appendix](../research/Research-Appendix-v1-full-text.md)
- [User journey map](../design/Speak-Back-User-Journey-Map.md)
- [UAT test cases and results](UAT-Test-Cases.csv)
- [Portfolio case study](../portfolio/Speak-Back-Case-Study.md)
- [Interactive Figma prototype](https://www.figma.com/design/PjPuEXfLOmN1UfnXrM6uVc/Duolingo---Speak-Back-Prototype-v1?node-id=0-1)

---

**Speak Back — Learn it. Say it. Share it.**  
Hriday Patel · Independent portfolio project · 2026
