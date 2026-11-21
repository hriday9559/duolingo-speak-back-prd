# Speak Back: Peer Speaking Practice for Duolingo

**A portfolio PRD by Hriday Patel**

*This is a student portfolio project. I am not affiliated with Duolingo. All Duolingo facts come from public sources, listed at the end.*

**Status:** Draft v0.2. User research is in progress, so evidence slots are still empty.
**Last updated:** 19 November 2026
**Research appendix:** survey, interview script and analysis method are in a separate document (Appendix).

> **How to read this document**
> - `[RESEARCH: ...]` = a slot for my own survey or interview findings, written as "X of N".
> - `[ASSUMPTION]` = something I believe but have not proven.
> - `[TARGET - to validate]` = a goal number, with the reasoning next to it.
> - `[UNVERIFIED]` or "verify this" = a public claim I could not confirm from an official source.
> - `[S1]`, `[S2]`... = sources, listed at the end.

---

## What I learned / what changed

*To be filled in after research.*

- **What I believed before research:** [fill in]
- **What the survey showed** (N = __): [RESEARCH: top 2–3 findings in "X of N" form]
- **What the interviews showed** (N = __): [RESEARCH: top 2–3 themes, with how many people raised each]
- **What I changed in this PRD because of it:** [fill in, e.g., a persona, a priority, the chosen option]
- **What I still don't know:** [fill in]

---

## 1. TL;DR

Many Duolingo learners may keep long streaks but still not feel able to hold a real conversation [RESEARCH]. Duolingo's social features help people *show up*, not *speak*, and its AI speaking tool, Video Call, is for paying subscribers only. Speak Back lets learners trade short, prompted voice replies with friends, tied to their Friend Streak, so speaking with a real person becomes part of the daily habit.

---

## 2. Background and problem statement

### 2.1 Duolingo today (public numbers)

From Duolingo's Q3 2026 shareholder letter [S1]:

| Metric | Q3 2026 | Notes |
|---|---|---|
| Daily active users (DAUs) | 64.9M | Average over the quarter. Up 29% year on year. |
| Monthly active users (MAUs) | 153.1M | Average over the quarter. Up 13% year on year. |
| Paid subscribers | 13.1M | Count at the end of the period. |
| Paid subscribers ÷ MAUs | **about 8.6%** | My own calculation, an approximation. One number is a period-end count; the other is a quarterly average. The letter does not state this figure. |

**Takeaway:** roughly 9 in 10 monthly learners do not pay. So any feature locked to paid plans misses most learners.

### 2.2 What Duolingo already has (checked 19 Nov 2026)

| Feature | Exists? | What it does | What it does NOT do | Source |
|---|---|---|---|---|
| **Friend Streak** | Yes (launched Aug 2024) | Share a streak with friends (up to 5 at launch; verify this is still the limit). Both must do a lesson each day. You can nudge a friend. | No speaking. It rewards doing a lesson, not talking. | [S2], [S3] |
| **Friends Quests** | Yes | Weekly. Duolingo pairs you with one mutual friend to hit a shared goal (e.g., XP) in 5 days. | No speaking. You can't pick the partner. Mobile only. | [S4] |
| **Video Call** (AI conversation practice) | Yes, **paid subscribers only** | Real-time spoken chat with an AI character. Duolingo says it is giving unlimited Video Call to new Super subscribers and is "on track to make it available to all Super subscribers by the end of this year" (2026). | Not a real human. No social accountability. Not for free learners. | [S1] |
| **Max tier** | **Being sunset** | Duolingo said it would stop selling new Max subscriptions in November 2026. Existing Max individual subscribers move to a Super family plan at the same price. | — | [S1] |
| **More speaking exercises** | Yes | Duolingo says the share of exercises you can answer by speaking "has doubled" since the start of 2026. | Solo practice. You speak to the app, not to a person. | [S1] |
| **Duolingo Events** (live sessions with real people) | **Retired** (early 2023) | Was live group sessions. | No longer available. | [S5] (third-party blog; verify this with an official source) |
| **Stories** | Yes (verify this) | Short read-and-listen stories with questions. | Not speaking with a person. | No official source checked — verify this |
| **Leaderboards (Leagues)** | Yes (verify this) | Weekly XP competition with strangers. | No direct talk between learners. | No official source checked — verify this |

**What this tells us**

1. Duolingo's social features are about **accountability** (streaks, quests, leagues), not **conversation**.
2. Duolingo is clearly investing in speaking (more speaking exercises, Video Call for all Super subscribers). But all of it is **you and the app**. None of it is **you and another person**.
3. Duolingo tried live human sessions (Events) and retired them. This idea must explain why it is different (see Risks).
4. Duolingo has said learners with at least one Friend Streak are 22% more likely to do their daily lesson, and that 57% of users have at least one friend on the app [S3]. These are Duolingo's own 2024 claims. They may be out of date.

### 2.3 Problem statement

**Problem 1: The streak is not the skill.**
Learners may keep their streak but not feel able to speak or understand real conversation.
- [RESEARCH: __ of __ respondents who used Duolingo for 6+ months rated their speaking ability 1 or 2 out of 5]
- [RESEARCH: __ of __ interviewees described freezing or struggling in a real conversation]

**Problem 2: Learning is solo.**
Learners may want to practice with other people, but the app gives them no way to talk to each other.
- [RESEARCH: __ of __ respondents said they would like to practice with another learner]
- [RESEARCH: __ of __ lapsed respondents picked "wanted to practice real conversation" as a reason they stopped]

**One-line problem statement:**
*Duolingo learners who are building a daily habit have no low-pressure way to speak with a real person, so their confidence in real conversation may not grow with their streak.*

---

## 3. Hypotheses and how I'll validate them

| # | Hypothesis | How I'll test it | Supported if... |
|---|---|---|---|
| H1 | Many long-time learners rate their speaking ability low. | Survey: time used × speaking self-rating | [TARGET - to validate] About 4 in 10 users of 6+ months rate speaking 1–2 out of 5. Reasoning: below that, the problem may be too small to prioritize. |
| H2 | Learners are open to practicing with other learners. | Survey + interviews | [TARGET - to validate] About 3 in 10 say "Would like it." Reasoning: new social features usually start with a minority. |
| H3 | Friends feel safer than strangers. | Survey (worries, preferred format) + interviews | "Friend" options beat "stranger" options, and safety or strangers are common worries. |
| H4 | Voice messages are easier to start than live calls. | Survey (preferred format) + interviews; later a fake-door test | Voice-message options get more picks than live-call options. |
| H5 | Speaking with a friend improves retention without hurting lessons. | Only an A/B test can show this (Section 10) | Higher 28-day retention, no drop in daily lesson completion. |

**Note on sample size:** My research is small (target 50+ survey responses, 5–6 interviews). It can show *direction*, not proof. H1–H4 results will be reported as "X of N" and treated as signals. H5 needs a real experiment at scale.

---

## 4. Goals and non-goals

**Goals**
1. Give learners a way to practice speaking with a real person, including free learners.
2. Make speaking part of the existing daily habit (Friend Streak).
3. Increase learners' confidence in speaking.
4. Increase long-term retention.

**Non-goals (this version)**
1. Live voice or video calls between learners.
2. Matching with strangers.
3. Replacing Video Call. AI practice and friend practice do different jobs.
4. Scoring speech accuracy.
5. Tutors or teachers.
6. Making money directly. This is an engagement and retention feature first.

---

## 5. Personas (hypotheses until my research confirms them)

### Persona 1: "Streak-Keeper Priya" [ASSUMPTION]
- 21, engineering student in Pune. Learning Spanish for 14 months. Long streak.
- Does one lesson at night, often an easy one, to save the streak.
- Has a few Duolingo friends from college.
- **Pain:** knows many words but freezes when speaking [RESEARCH: replace with a real pattern from interviews].
- **Wants:** proof she can really speak; low-pressure practice.
- **Won't do:** talk to strangers; pay for a subscription.

### Persona 2: "Lapsed Social Learner Arjun" [ASSUMPTION]
- 26, works in sales in Bengaluru. Learned French for 4 months, then stopped.
- Learns best with people.
- **Pain:** the app felt like a game played alone [RESEARCH: replace with a real pattern from interviews].
- **Wants:** someone to practice with; a reason to come back.
- **Won't do:** commit to fixed-time live classes.

---

## 6. User stories and acceptance criteria

| # | User story | Acceptance criteria |
|---|---|---|
| US1 | As a learner, I want to send a short voice reply to a friend using a prompt, so I can practice speaking without pressure. | Can pick a mutual friend. Prompt matches my course level. Record up to 60 seconds, listen back, re-record, send. Friend is notified. |
| US2 | As a learner, I want to hear and answer my friend's voice reply, so we have a back-and-forth. | Play at 1× or 0.75×. See the prompt they answered. Reply by voice in the same thread. Send one of 3 preset reactions. |
| US3 | As a learner with a Friend Streak, I want speaking to show on our streak, so it becomes part of my habit. | A completed exchange (both sides sent) shows a "spoke today" badge. It does **not** replace the daily lesson in v1. |
| US4 | As a nervous learner, I want hints before I speak, so I don't freeze. | Each prompt shows 3 helpful phrases and an optional example answer. |
| US5 | As a learner, I want to report, block and control who can message me, so I feel safe. | Report and block in 1 tap from any message. Only mutual followers can exchange. Feature can be turned off. Hidden for users under the regional minimum age. |
| US6 | As a learner, I want to hear my progress over time. | List of past recordings by date. Play first and latest side by side. |

---

## 7. Solution options and RICE scoring

**RICE** = (Reach × Impact × Confidence) ÷ Effort.
- **Reach:** relative score 1–10 (I don't have Duolingo's internal data).
- **Impact:** 0.25 (tiny) to 3 (massive).
- **Confidence:** how sure I am.
- **Effort:** person-months.

**All values are [ASSUMPTION], for comparison only.**

| Option | Description | Reach | Impact | Confidence | Effort | **RICE** |
|---|---|---|---|---|---|---|
| **A. Async voice with friends ("Speak Back")** | Prompted voice replies between mutual friends, linked to Friend Streak. | 6 | 2 | 60% | 4 | **1.8** |
| **B. Live 1:1 calls with matched strangers** | Real-time voice call with a learner at the same level; AI suggests topics. | 8 | 3 | 30% | 10 | **0.72** |
| **C. Live group speaking rooms** | Scheduled group rooms with a host. | 3 | 2 | 20% | 8 | **0.15** |

**Why these scores**
- **A:** Reach is limited to people with friends on the app, but confidence is highest. It reuses the friend graph and Friend Streak. It avoids strangers and time zones.
- **B:** Biggest potential impact, but hard problems: matching, cold start, real-time moderation and safety. Much more work.
- **C:** Lowest. Duolingo already ran live Events and retired them [S5].

**Decision: Option A.**

**Trade-offs I accept**
- A voice message is not a live conversation. But it tests the core question cheaply: *will learners speak to each other at all?*
- Users with no friends on the app are left out at first. Invite links and stranger matching come later.
- Replies can be slow. I'll track reply time and use nudges.

**Why not just rely on Video Call?**
Video Call is good AI practice, and Duolingo is expanding it to all Super subscribers [S1]. But two gaps remain:
1. **It's for paying users only.** Roughly 9 in 10 monthly learners don't pay [S1], so they can't use it.
2. **AI is not a person.** It doesn't give you a real human voice, real accents and mistakes, or a friend who is counting on you to reply.

Speak Back's difference is the **real human and friend element**, not price. Paying users benefit too. The two can work together: Video Call to warm up, Speak Back to use it with a real person.

---

## 8. Requirements

**P0 (must have for launch)**
1. Send a prompted voice reply (up to 60 seconds) to a mutual friend.
2. Receive, play (1× and 0.75×) and reply in a thread.
3. Prompt library matched to each learner's course level.
4. Hints: 3 phrases and an example answer per prompt.
5. Report, block and mute on every message. Feature on/off in settings.
6. Mutual followers only. No strangers.
7. Age gate by region [ASSUMPTION: confirm minimum ages with legal].
8. Automated screening (speech-to-text plus content filter) before delivery. Human review for reported messages.
9. "Spoke today" badge on Friend Streak after a completed exchange.
10. Analytics events for every metric in Section 9.

**P1 (soon after launch)**
1. Push nudge: "Your friend sent you a Speak Back."
2. Speaking history (first vs latest).
3. Preset reactions ("Nice!", "I understood you!", "Say it again?").
4. Auto transcript so the listener can read along.
5. Invite link to bring a friend onto Duolingo.

**P2 (later)**
1. AI tips on your recording.
2. Opt-in matching with a stranger at the same level, after safety metrics are healthy.
3. Short live calls with friends.
4. Speak Back challenges inside Friends Quests.

---

## 9. Success metrics

### North Star: Weekly Speaking Learners (WSL)
- **Definition:** learners who completed at least one full exchange in the last 7 days.
- **Full exchange:** they sent a voice reply **and** received one back in the same thread.
- **Calculation:** count of distinct users with sent ≥ 1 and received ≥ 1 in the last 7 days.
- **Why:** it counts two-way speaking, not just recording into the void.
- **Target:** [TARGET - to validate] 5% of eligible users (those with ≥1 mutual friend) within 8 weeks. Reasoning: new opt-in social features start small; 5% is a realistic first bar.

### Input metrics

| Metric | Calculation | Target |
|---|---|---|
| **Send rate** | Users who sent ≥1 voice reply ÷ users who saw the entry point, per week | [TARGET - to validate] 15%. Speaking to a friend is a big step, so most viewers won't try it at first. |
| **24-hour reply rate** | Replies received within 24h ÷ voice replies sent | [TARGET - to validate] 40%. If most messages go unanswered, senders give up. |
| **Exchanges per speaking learner per week** | Completed exchanges ÷ WSL | [TARGET - to validate] 2+. One exchange may be curiosity; two suggests a habit. |

### Guardrail metrics (must not get worse)

| Guardrail | Calculation | Threshold |
|---|---|---|
| **Daily lesson completion rate** | Users completing ≥1 lesson today ÷ DAU | No statistically significant drop vs control. |
| **Reports per 1,000 exchanges** | (Messages reported ÷ messages sent) × 1,000 | [TARGET - to validate] Below 2. Friends-only should be low-risk; higher means safety design is failing. Pause rollout if crossed. |
| **Friend Streak break / unfollow rate** | Friend Streaks broken (or unfollows) ÷ active Friend Streaks, per week | No significant rise vs control. |

---

## 10. Experiment plan (A/B test)

**The challenge:** this is a social feature. If I'm in the test group and my friend is in control, I can't send them anything. This is called **network interference**.

**The fix: cluster randomization.** Group users into friend clusters (people linked by mutual follows). Assign whole clusters to test or control.

| Item | Plan |
|---|---|
| **Eligible users** | 18+ (or regional minimum age), mobile, ≥1 mutual friend, in 3–5 languages with prompts ready. Free and paid. |
| **Control** | Current app. |
| **Treatment** | Speak Back (P0 + push nudge). |
| **Split** | 50/50 by friend cluster. Start with about 5% of eligible users. |
| **Primary metric** | 28-day retention (active on day 28 after entering the test). |
| **Secondary** | WSL, input metrics, and a one-question in-app speaking-confidence check at day 21. |
| **Guardrails** | The three in Section 9. |
| **Duration** | At least 4 full weeks. Behavior varies by weekday, 28-day retention needs 28 days, and early excitement (the novelty effect) fades. |
| **Smallest effect worth detecting** | [TARGET - to validate] +1 percentage point in 28-day retention. At Duolingo's scale, 1 point is many retained learners. |
| **Sample size** | Use a standard calculator with: baseline 28-day retention [ASSUMPTION: not public], the effect above, 95% confidence, 80% power. Then increase it, because clusters reduce the effective sample. |

**Risks to validity**
1. **Spillover:** friendships cross clusters. Measure how many.
2. **Novelty effect:** look at weeks 3–4 on their own.
3. **Selection bias:** only users with friends are eligible. Results don't apply to solo learners.
4. **Seasonality:** avoid exam season and New Year spikes.
5. **Gaming:** count a reply only if it's ≥5 seconds with detected speech.

---

## 11. Risks and mitigations

| Risk | Why it matters | Mitigation |
|---|---|---|
| **Safety / harassment** | Voice can carry abuse. Spam and inappropriate messages are reported as a common complaint on HelloTalk [S9] (competitor-written source). | Friends-only. 1-tap report and block. Age gate. Clear rules shown before the first send. |
| **Moderating voice** | Harder than text. | Speech-to-text screening before delivery. Human review of reports. Limited storage time [ASSUMPTION: set with legal]. |
| **Privacy and law** | Voice is personal data. India's DPDP Act and GDPR may apply [UNVERIFIED: confirm specifics with legal]. | Clear consent. Easy deletion. Store as little as possible. |
| **Matching quality** | Friends may be at different levels or learning different languages. | Prompts adapt to each person's level. Show each friend's language. Suggest friends learning the same language. |
| **Cold start** | The feature needs active friends to work. | Launch only to users with ≥1 active mutual friend. Invite links (P1). Strangers later (P2). |
| **Embarrassment** | Users may never press record. | Hints, example answers, listen-back before sending, kind preset reactions, no public scores. |
| **Events was retired** | Duolingo tried live human sessions and stopped. | Speak Back is async, friends-only and inside the daily loop, not scheduled. Still an open question. |
| **Hurts core learning** | People may swap a lesson for a voice message. | Doesn't count as the lesson in v1. Lesson-completion guardrail. |

---

## 12. Rollout and roadmap

**Dependencies:** friends graph and Friend Streak; audio storage and playback; speech-to-text per language; Trust & Safety rules and review staff; learning designers for prompts; legal and privacy review; notifications; data team for cluster randomization.

**Rollout**

| Phase | Who | Gate to move on |
|---|---|---|
| 0. Internal testing | Employees | No major bugs. Moderation pipeline works. |
| 1. Fake-door test | Small % see a "Speak Back — coming soon" card | [TARGET - to validate] ≥5% tap rate shows real interest. |
| 2. A/B test | ~5% of eligible users, 3–5 languages | Primary metric up; guardrails hold. |
| 3. Expand | 25% → 50% → 100% of eligible users | Report rate under threshold; systems stable. |
| 4. More languages | Remaining courses | Prompts and speech-to-text ready. |

**Roadmap**

| **Now** (0–3 months) | **Next** (3–6 months) | **Later** (6–12+ months) |
|---|---|---|
| User research | Transcripts, speaking history, reactions, invite links | Opt-in stranger matching by level |
| Fake-door test | Speak Back challenges in Friends Quests | Short live calls with friends |
| P0 build + A/B test | "Warm up with Video Call, then Speak Back" flow for Super subscribers | Group speaking circles (only if data supports it) |

---

## 13. Open questions

1. Why exactly was Duolingo Events retired? What applies here? [RESEARCH — verify this]
2. What share of active friendships are in the same language? This sets real reach.
3. Should a completed exchange ever count toward the streak, or only show a badge?
4. Do learners prefer friends, or do they really want native speakers?
5. What does voice moderation cost per 1,000 messages?
6. Does Speak Back change Super conversion, positively (people want more speaking practice) or not at all?
7. What is the minimum age for voice features in each region?

---

## 14. Competitive teardown

| | **Duolingo** | **Babbel** | **Speak** | **HelloTalk** (peer practice) |
|---|---|---|---|---|
| **Model** | Free core app; paid Super plan [S1]. | Paid courses. | AI speaking tutor; paid tiers [S8]. | Free language exchange; paid VIP [S9]. |
| **Speaking** | Speaking exercises; Video Call (AI) for Super subscribers [S1]. | Babbel Speak: AI conversation, beta, free for registered users, 4 languages [S6]. Live classes with teachers, up to 6 students (launched 2021) [S7] (verify current status). | AI roleplay and free talk [S8]. | Text, voice notes and calls with real people [S9]. |
| **Real humans?** | No (Events retired [S5]) | Yes, paid teachers | No (AI) | Yes, other users |
| **Strengths** | Habit and motivation; very large user base [S1]; strong friend features [S2][S4]. | Clear grammar teaching; real teachers. | Accurate speech recognition; engaging roleplay; polished app [S8]. | Native speakers; in-chat corrections; large community (claims 70M+ registered users, self-reported) [S9]. |
| **Weaknesses** | No way to speak with other people. AI speaking is paid only. | Live classes cost extra [S7]; less social [ASSUMPTION]. | Brief feedback; recognition can be too lenient; repetitive at higher levels [S8] (reviewer is a competitor). | Spam and unwanted messages are a common complaint [S9] (competitor-written); hard for beginners to keep a chat going [ASSUMPTION]. |

**Tandem**, similar to HelloTalk, claims 30M+ users and is described as having stricter moderation, video calls and events [S9]. Source is a competitor's blog, so treat as [UNVERIFIED].

**The gap:** AI apps give safe practice but no human connection. Exchange apps give humans but are unstructured, risky with strangers, and hard for beginners. **No product in this table combines structured prompts, real people you already know, safety, and a daily habit** [ASSUMPTION: based on the features above; I will verify by using each app].

---

## 15. Prototype spec (6 screens)

Build in Figma. Use a friendly, rounded style. **Do not use Duolingo's logo, mascot or characters.**

### Screen 1: Home with Speak Back card
- **Purpose:** entry point where learners already are.
- **Elements:** learning path in background. Card: mic icon, "Speak Back", "Practice speaking with Priya today", friend avatar, Friend Streak flame and day count.
- **Buttons:** `Start` → Screen 2. `✕` → hide card for today.

### Screen 2: Choose a friend
- **Purpose:** pick who to speak with.
- **Elements:** "Who do you want to practice with?" List of mutual friends: avatar, name, language flag, level, Friend Streak days. Friends learning another language are greyed out ("Learning French").
- **Buttons:** tap a friend → Screen 3. `Invite a friend` → share sheet (P1). `←` → Screen 1.

### Screen 3: Prompt and hints
- **Purpose:** reduce fear before speaking.
- **Elements:** prompt in target language with English below (e.g., "¿Qué hiciste el fin de semana? / What did you do at the weekend?"). 3 "Helpful words" chips. Collapsible "See an example answer." Note: "Your friend will hear this. Be kind."
- **Buttons:** `Shuffle prompt` → new prompt at the same level. `I'm ready` → Screen 4.

### Screen 4: Record and review
- **Purpose:** record, listen back, send.
- **Elements:** big mic button, timer "0:00 / 1:00", live waveform, playback bar after recording.
- **Buttons:** `Hold to record` → records while held. `Play` → plays it back. `Re-record` → clears. `Send to Priya` → toast "Sent! We'll tell you when Priya replies." → Screen 5.
- **Rule:** under 5 seconds shows "Try saying a little more" and disables Send.

### Screen 5: Conversation thread
- **Purpose:** see the back-and-forth.
- **Elements:** messages with avatar, prompt label, audio bubble, duration, `1×`/`0.75×` toggle, transcript link (P1), reactions. Top banner after a full exchange: "You both spoke today 🔥 Friend Streak: 42 days."
- **Buttons:** `Play`; `0.75×`; reaction chips `Nice!` / `I understood you!` / `Say it again?`; `Reply with voice` → Screen 4 with the same prompt; `⋯` → Screen 6.

### Screen 6: Safety sheet
- **Purpose:** fast, clear safety controls.
- **Elements:** bottom sheet, "Keep Speak Back friendly and safe."
- **Buttons:** `Report this message` → pick reason → `Submit` → "Thanks. We'll review this." `Block Priya` → confirm `Block` / `Cancel`. `Mute Speak Back from Priya`. `Turn off Speak Back` → Settings. `Cancel`.

**Flow:** 1 → 2 → 3 → 4 → 5 → (⋯) 6, plus a "friend replied" notification that opens Screen 5.

---

## Sources

- **[S1]** Duolingo, Q3 2026 Shareholder Letter (3 Nov 2026), SEC filing: DAUs, MAUs, paid subscribers, Video Call for Super subscribers, Max sunset, speaking exercises. https://www.sec.gov/Archives/edgar/data/0001562088/000162828026069474/q3fy26duolingo9-30x26share.htm
- **[S2]** Duolingo Blog, "Friend Streak" (5 Aug 2024). https://blog.duolingo.com/friend-streak/
- **[S3]** Duolingo Blog, "Product lessons from Friend Streak" (Sep 2024, updated Feb 2025). The 22% and 57% figures are Duolingo's own claims from that time. https://blog.duolingo.com/product-lessons-friend-streak/
- **[S4]** Duolingo Blog, "Friends Quests" (2022, updated June 2026). https://blog.duolingo.com/friends-quests/
- **[S5]** Third-party blog on Duolingo Events retiring (Feb 2023). Not official; verify this. https://rebeccasdaf.substack.com/p/duolingo-events-retired-but-mine
- **[S6]** Babbel, Conversation practice / Babbel Speak (page accessed Nov 2026). https://www.babbel.com/babbel-conversation-practice
- **[S7]** TechCrunch, "Babbel adds live classes, games and more" (2 Feb 2021). May be out of date. https://techcrunch.com/2021/02/02/language-learning-service-babbel-adds-live-classes-games-and-more/
- **[S8]** Languatalk, "Speak App Review" (updated Nov 2026). Written by a competitor; treat as opinion. https://languatalk.com/blog/speak-app-review/
- **[S9]** TalkDrill, "HelloTalk vs Tandem" (updated Oct 2026). Written by a competitor; user counts are self-reported. https://www.talkdrill.com/blog/compare/hellotalk-vs-tandem/