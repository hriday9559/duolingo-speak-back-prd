# Duolingo "Speak Back": Peer Speaking Practice — Portfolio PRD

**Author:** Manish (portfolio project, not affiliated with Duolingo)
**Status:** Draft v0.1. Research not yet run. All evidence slots are placeholders.
**Last updated:** 19 Nov 2026

> **How to read this document**
> - `[RESEARCH: ...]` = a slot you must fill with your own survey or interview data.
> - `[ASSUMPTION]` = something I believe but have not proven.
> - `[TARGET - to validate]` = a goal number. The reasoning is given next to it.
> - `[UNVERIFIED]` / "verify this" = a public claim I could not confirm from a primary source.
> - Every public number has a source link in the **Sources** section at the end.

---

## Step 0: What Duolingo already has (checked 19 Nov 2026)

Rule 2 says: check before proposing. Here is what I found.

| Feature | Exists? | What it does | What it does NOT do | Source |
|---|---|---|---|---|
| **Friend Streak** | Yes (launched Aug 2024) | Share a streak with up to 5 friends. Both must do a lesson each day. You can nudge a friend. | No speaking. It rewards *doing a lesson*, not *talking*. | [S1], [S2] |
| **Friends Quests** | Yes (since 2022) | Weekly. Duolingo pairs you with one mutual friend. You hit a shared goal (e.g., XP) in 5 days. | No speaking. You can't pick the partner. Mobile only. | [S3] |
| **Video Call (with Lily, an AI character)** | Yes, **Duolingo Max only** | Real-time spoken chat with an AI. Transcripts. "Lily Calls You." | Not a real human. Paid tier only. Limited languages. | [S4] |
| **Duolingo Events** (live group sessions with real people) | **Retired** (sunset announced Dec 2022, ended Jan 2023) | Was live online and in-person sessions. | No longer available. | [S5] (third-party blog; verify this with an official Duolingo source) |
| **Stories** | Yes (verify this) | Short read-and-listen stories with comprehension questions. | Listening/reading, not free speaking with a person. | No primary source fetched — verify this |
| **Leaderboards (Leagues)** | Yes (verify this) | Weekly XP competition in groups of strangers. | Competition only. No direct talk between learners. | No primary source fetched — verify this |

**What this tells us**

1. Duolingo's social system is about **accountability** (streaks, quests, leagues). It is not about **conversation**.
2. Speaking practice exists, but only with **an AI**, and only for **paying Max users**.
3. Duolingo **tried live human sessions (Events) and retired them**. Any peer-speaking idea must explain why it would work where Events did not. I return to this in Risks and Interview Prep.
4. Duolingo says learners with at least one Friend Streak are **22% more likely** to do their daily lesson, and **57%** of users have at least one friend on the app [S2]. This is Duolingo's own claim, not an audited number. But it suggests the friend graph is large and that social features move behavior.

**My refined idea:** Don't build "live calls with strangers" first. Build **asynchronous voice exchanges between friends**, with structured prompts, tied to Friend Streak. ("Asynchronous" = not at the same time, like voice notes on WhatsApp.) Then add live practice and stranger matching later, only if the data supports it. The reasoning is in Part C, Section 7.

---

# Part A: Research kit

## A1. Survey (10 questions)

**Who:** Anyone who has used Duolingo for at least one week, now or in the past.
**Where to share:** College WhatsApp groups, LinkedIn, r/duolingo (check subreddit rules), language clubs.
**Goal sample:** At least 100 responses. Fewer than 50 is too small to split into groups.
**Time to fill:** About 4 minutes.

> Tip: Keep the order below. Usage questions come first, so people answer them before they think about "my feature."

| # | Question | Type | Options | Tests |
|---|---|---|---|---|
| 1 | Which language(s) have you studied on Duolingo? | Multi-select | List + "Other" | Segmenting |
| 2 | In total, how long have you used Duolingo? | Single choice | < 1 month / 1–3 months / 3–12 months / 1–2 years / 2+ years | Segmenting |
| 3 | Which best describes you today? | Single choice | I use it most days / I use it sometimes / I stopped using it / I've never stopped but I'm thinking about it | Churn |
| 4 | (If stopped or thinking about it) What were the main reasons? Pick up to 3. | Multi-select | Got bored / Too easy / Too hard / No time / Didn't feel I was improving / Wanted to practice real conversation / Lost my streak / Switched to another app / Other (write in) | Both problems (options mixed, not leading) |
| 5 | How would you rate your ability to hold a simple 2-minute conversation in that language with a native speaker today? | Scale 1–5 | 1 = Could not at all, 5 = Could easily | Problem 1 |
| 6 | How would you rate your ability to understand people speaking at normal speed (e.g., a video or a person)? | Scale 1–5 | 1 = Understand almost nothing, 5 = Understand almost everything | Problem 1 |
| 7 | In the last month, how did you practice speaking the language, if at all? Pick all that apply. | Multi-select | Duolingo speaking exercises / Duolingo Video Call / Talked with a friend or family / Language exchange app / Tutor or class / I did not practice speaking / Other | Problem 1 + 2 (current behavior) |
| 8 | How do you feel about speaking the language with another learner at a similar level? | Single choice | Would like it / Neutral / Would not like it / Not sure | Problem 2 |
| 9 | (If "Would not like it" or "Not sure") What would worry you? Pick all that apply. | Multi-select | Feeling embarrassed / Safety or privacy / Partner's level too different / Scheduling / Talking to strangers / Prefer AI / Prefer to stay solo / Other | Problem 2 barriers |
| 10 | If you could practice speaking with someone on Duolingo, which would you be most likely to try? | Single choice | Live call with a friend / Live call with a matched stranger / Voice messages with a friend / Voice messages with a matched stranger / None of these | Solution direction |

**Optional last field:** "Can we contact you for a 15-minute interview?" (email or phone). Say clearly how you will use it.

**Why these questions are not leading**
- Q4 mixes many reasons. "Real conversation" is one option among nine.
- Q5 and Q6 use a neutral scale. They don't say "Do you struggle to...".
- Q8 offers "Would not like it" as a real option and Q9 explores why.

## A2. Interview script (15 minutes, 7 questions)

**Who:** 8–12 people from the survey. Pick a mix: 3–4 active users, 3–4 who stopped, 2–3 who use another speaking app.
**Rules for you:** Ask about past behavior, not future wishes. Don't pitch the idea until the last question. Stay quiet after they answer. Record only with permission.

| Time | Question | Follow-up probes |
|---|---|---|
| 0–1 min | **Intro.** "Thanks for your time. I'm a student studying how people learn languages. There are no right answers. Can I take notes?" | — |
| 1–3 | **Q1.** "Tell me how you started using Duolingo. Why that language?" | "What did you hope to be able to do?" "Has that goal changed?" |
| 3–5 | **Q2.** "Walk me through the last time you used Duolingo. What did you do?" | "What time of day?" "What made you open it?" "Was it for the streak or for learning?" |
| 5–7 | **Q3.** "Tell me about a time you tried to actually use the language with a real person." | "What happened?" "How did it feel?" "What was hardest — speaking or understanding?" |
| 7–9 | **Q4.** "How, if at all, do you practice speaking today?" | "Why that way?" "What stops you from doing more?" "Have you tried Video Call or any other app?" |
| 9–11 | **Q5.** "Have you ever practiced with another learner or a language partner? Tell me about it." | "How did you find them?" "Why did it stop or continue?" "Anything uncomfortable?" |
| 11–13 | **Q6.** (Only if they stopped) "What was going on when you stopped using Duolingo?" | "Was there a moment you decided?" "What would have made you stay?" |
| 13–15 | **Q7.** (Concept check, last) "Imagine you could send a short voice reply to a friend on Duolingo, using a prompt like 'Describe your weekend.' What would you think?" | "When would you use it?" "What would make you not use it?" "Friend or stranger? Why?" |
| End | "Is there anything I should have asked but didn't?" | Thank them. |

## A3. How to analyze the responses

**Survey (numbers)**
1. Clean the data. Remove blank and joke answers. Write down how many you removed.
2. Make three segments from Q3: **Active**, **Lapsed** (stopped), **At-risk** (thinking of stopping).
3. For each segment, count:
   - % who picked each reason in Q4.
   - Average and spread of Q5 and Q6 (speaking and listening confidence).
   - % who say "Would like it" in Q8.
4. Cross-tab Q2 (how long used) with Q5. This tests Problem 1: *Do long-time users still rate speaking low?*
5. Report as "**X of N** respondents" plus the %. Never only %. Small samples mislead.

**Interviews (words) — affinity clustering**
1. After each interview, write each distinct point on its own sticky note (Miro or FigJam works). One idea per note.
2. Put all notes on one board. Group similar ones. Name each group with a short user-voice phrase, for example "I freeze when someone talks fast."
3. Count how many **different people** mention each group (not how many notes).
4. Rank the groups by people count, then by how strongly people felt.
5. Mark each group as supporting Problem 1, Problem 2, both, or neither.

**Decide**
- Write a one-line verdict for each hypothesis: **Supported / Weak / Not supported**.
- If Problem 2 is "Not supported," say so in the PRD and change direction. This shows real product thinking.

---

# Part B: Competitive teardown

| | **Duolingo** | **Babbel** | **Speak** | **HelloTalk** (peer-practice) |
|---|---|---|---|---|
| **Core model** | Free, gamified, short lessons. Paid tiers (Super, Max). | Paid, structured courses. | AI speaking tutor. Paid. | Free language exchange with native speakers. Paid VIP. |
| **Speaking practice** | Speaking exercises in lessons. Video Call with AI, Max only [S4]. | "Babbel Speak": AI conversation, beta, free for registered users, 4 languages [S7]. Live classes with real teachers, max 6 students, launched 2021 [S8] (current pricing: verify this). | Core product: AI roleplay and free talk [S9]. | Text, voice notes, calls with real people [S10]. |
| **Real humans?** | No (Events retired [S5]) | Yes, paid teachers (Live) | No (AI); a tutor option is mentioned [S9] (verify this) | Yes, other users |
| **Does well** | Habit and motivation. Huge user base: 50.5M DAUs, 135.3M MAUs in Q3 2025 [S6]. Strong friend graph [S2]. | Clear grammar teaching. Real teachers. | Accurate speech recognition. Engaging roleplay. Polished UI [S9]. | Real native speakers. In-chat corrections. Huge community: claims 70M+ registered users [S10] (self-reported). |
| **Does badly** | Speaking with people is missing. AI speaking is paywalled. Critics say the streak rewards habit more than skill [ASSUMPTION — validate in research]. | Live classes cost extra. Less fun and less social [ASSUMPTION]. | Feedback is brief. Recognition can be too lenient. Repetitive at higher levels [S9] (reviewer is a competitor). | Spam and inappropriate messages are a common complaint [S10] (competitor-authored). Shows personal info by default (2021 review) [S11]. Hard for beginners to keep a chat going [ASSUMPTION]. |
| **Price** | Free core; Super and Max paid (verify current prices) | Subscription (verify) | Premium / Premium Plus (prices not stated in source) [S9] | VIP $6.99/month or $45.99/year [S10] (verify) |

**Note on Tandem:** Tandem is similar to HelloTalk. It claims 30M+ users and is described as having stricter moderation, video calls and events [S10]. That source is a competitor's blog, so treat it as [UNVERIFIED].

### The gap my idea could fill

- **AI apps** (Speak, Video Call) give safe practice but **no real human connection or social accountability**.
- **Exchange apps** (HelloTalk, Tandem) give real humans but are **unstructured, risky with strangers, and hard for beginners**.
- **Duolingo has the friend graph and the habit loop**, but no way to *talk* to those friends.

**Gap:** *Structured, safe, beginner-friendly speaking practice with people you already know, built into a daily habit.* No product in this table combines all four [ASSUMPTION — based on the features listed above; verify by using each app yourself].

---

# Part C: The PRD

## 1. TL;DR

Many Duolingo learners may keep long streaks but still can't hold a real conversation [RESEARCH]. Duolingo's social features help people *show up*, but not *speak*, and its AI speaking tool is only in the paid Max tier. "Speak Back" lets learners trade short, prompted voice replies with friends, tied to their Friend Streak, so speaking with a real person becomes part of the daily habit.

## 2. Background and problem statement

**Background**
- Duolingo is large and growing: 50.5M daily active users and 135.3M monthly active users in Q3 2025 [S6].
- Only about 9% of monthly users pay [S6]. So most learners can't use Video Call, the main speaking feature [S4].
- Duolingo says 57% of users have at least one friend, and Friend Streaks make people 22% more likely to do their daily lesson [S2].

**Problem 1: The streak is not the skill.**
Learners keep their streak, but many may not feel able to speak or understand real conversation.
- Evidence: [RESEARCH: __ of __ respondents who used Duolingo for 6+ months rated their speaking ability 1 or 2 out of 5]
- Evidence: [RESEARCH: __ of __ interviewees described freezing or failing in a real conversation]

**Problem 2: Learning is solo.**
Learners may want to practice with other people, but the app gives them no way to talk.
- Evidence: [RESEARCH: __ of __ respondents said they would like to practice with another learner]
- Evidence: [RESEARCH: __ of __ lapsed users named "wanted to practice real conversation" as a reason they stopped]

**Problem statement (one line):**
*Free Duolingo learners who are building a daily habit have no low-pressure way to practice speaking with a real person, so their confidence in real conversation may not grow with their streak.*

## 3. Hypotheses and how I'll validate each

| # | Hypothesis | How I'll test it | It's supported if... |
|---|---|---|---|
| H1 | Many long-time learners rate their speaking ability low. | Survey Q2 × Q5 cross-tab | [TARGET - to validate] At least 40% of 6+ month users rate speaking 1–2/5. Reasoning: if fewer than ~4 in 10 feel stuck, the problem may be too small to prioritize. |
| H2 | Learners are open to practicing with other learners. | Survey Q8, interview Q5 & Q7 | [TARGET - to validate] At least 30% say "Would like it." Reasoning: new social features usually reach a minority first; 30% is a cautious bar for a worthwhile segment. |
| H3 | Friends feel safer than strangers. | Survey Q9 + Q10, interviews | "Friend" options beat "stranger" options in Q10, and "talking to strangers" or "safety" are common worries in Q9. |
| H4 | Async voice is easier to start than live calls. | Survey Q10, interview Q7, and a fake-door test later | Voice-message options get more picks than live-call options in Q10. |
| H5 | Speaking with a friend increases retention without hurting lesson completion. | Only provable with an A/B test (Section 10) | Treatment group shows higher 28-day retention and no drop in daily lesson completion. |

## 4. Goals and non-goals

**Goals**
1. Give free learners a way to practice speaking with a real person.
2. Make speaking practice part of the existing daily habit (Friend Streak).
3. Increase learner confidence in speaking.
4. Increase long-term retention.

**Non-goals (for this version)**
1. Live video or voice calls. (Later, if data supports it.)
2. Matching with strangers. (Later, after safety tools are proven.)
3. Replacing Video Call with AI. This complements it. AI is good for "anytime" practice; peers are good for motivation and real voices.
4. Grading speech accuracy with a score. We'll give light feedback only.
5. Teacher or tutor marketplace.
6. Monetization. This is a free-tier engagement feature first.

## 5. Personas (hypotheses until validated)

> These personas are guesses. Update them after your interviews. Replace each `[RESEARCH]` slot with what real people said.

### Persona 1: "Streak-Keeper Priya" [ASSUMPTION]
- 21, engineering student in Pune. Learning Spanish for 14 months. 400-day streak.
- Does one lesson at night, often the easiest one, to save the streak.
- Has 3 Duolingo friends from college. Has a Friend Streak with one.
- **Pain:** "I know many words, but when I tried to speak on a trip, I froze." [RESEARCH: replace with a real quote pattern]
- **Wants:** Proof she can really speak. Low-pressure practice.
- **Won't do:** Talk to random strangers. Pay for Max.

### Persona 2: "Lapsed Social Learner Arjun" [ASSUMPTION]
- 26, works in sales in Bengaluru. Learned French for 4 months, then stopped.
- Learns better with people. Joined a French WhatsApp group once.
- **Pain:** "The app felt like a game I was playing alone. I got bored." [RESEARCH: replace with a real quote pattern]
- **Wants:** Someone to practice with. A reason to come back.
- **Won't do:** Commit to fixed-time live classes.

## 6. User stories with acceptance criteria

| # | User story | Acceptance criteria |
|---|---|---|
| US1 | As a learner, I want to send a short voice reply to a friend using a prompt, so I can practice speaking without pressure. | - I can pick a friend I follow mutually.<br>- I see a prompt matched to my course level.<br>- I can record up to 60 seconds, listen back, re-record, then send.<br>- Friend gets a notification. |
| US2 | As a learner, I want to listen and reply to my friend's voice message, so we have a back-and-forth. | - I can play their recording at 1× or 0.75× speed.<br>- I can see the prompt they answered.<br>- I can reply by voice in the same thread.<br>- I can react with one of 3 preset reactions. |
| US3 | As a learner with a Friend Streak, I want speaking exchanges to count toward our streak, so speaking becomes part of my habit. | - A completed exchange (both sides sent) shows a "spoke today" badge on the Friend Streak.<br>- It does **not** replace the lesson requirement in v1 (protects learning — see guardrails). |
| US4 | As a nervous learner, I want hints before I speak, so I don't freeze. | - Each prompt shows 3 example words or phrases.<br>- I can see an example answer (text) before recording. |
| US5 | As a learner, I want to block or report someone and control who can message me, so I feel safe. | - Report and block are reachable in 1 tap from any message.<br>- Only mutual followers can send voice replies.<br>- Speak Back can be turned off in settings.<br>- Users under the regional minimum age see no Speak Back (see Risks). |
| US6 | As a learner, I want to see my speaking history, so I can hear my progress. | - I see a list of my past recordings by date.<br>- I can replay my first and latest recording side by side. |

## 7. Solution options and RICE scoring

**RICE** = (Reach × Impact × Confidence) ÷ Effort. It's a simple way to compare ideas.
- **Reach:** how many users it touches per quarter. Here as a relative score, 1–10, because I don't have Duolingo's real data.
- **Impact:** 0.25 (tiny) to 3 (massive).
- **Confidence:** how sure I am, as %.
- **Effort:** person-months of work.

**All values below are [ASSUMPTION]. They are my estimates for comparison only.**

| Option | Description | Reach | Impact | Confidence | Effort | **RICE** |
|---|---|---|---|---|---|---|
| **A. Async voice with friends ("Speak Back")** | Prompted voice replies between mutual friends. Linked to Friend Streak. | 6 (friend graph is large [S2], only those with friends) | 2 | 60% | 4 | **1.8** |
| **B. Live 1:1 calls with matched strangers** | Real-time voice call with a learner at the same level. AI suggests topics. | 8 (anyone can use it) | 3 | 30% | 10 | **0.72** |
| **C. Live group speaking rooms** | Scheduled group rooms led by a host, like the old Events. | 3 (only those who can attend at set times) | 2 | 20% | 8 | **0.15** |

**How I got the numbers (short)**
- **A** has lower reach (needs a friend) but the highest confidence. It reuses the existing friend graph and the Friend Streak, and it avoids strangers and time zones.
- **B** has the highest potential impact but low confidence. It has hard problems: matching quality, cold start, real-time moderation and safety. It's also much more work.
- **C** scores lowest. Duolingo already ran live Events and retired them [S5]. I don't know why [RESEARCH: find any public statement on why Events was retired — verify this], but it is a warning sign.

**Pick: Option A.**

**Trade-offs I accept**
- **Less "real" than a live call.** Async voice is not a true conversation. But it's a safer first step and it tests the core question: *will people speak to each other at all?*
- **Smaller reach.** Users with no friends on the app are left out at first. Next phase: invite links and opt-in stranger matching.
- **Slower feedback loop.** Replies may take hours. We'll measure reply time and nudge.

**Why not just improve Video Call (AI)?** AI is great for practice, but it lacks two things a friend gives: social accountability, and a real human voice with real accents and mistakes. It is also in the paid tier [S4]. Speak Back serves free users. In the future, AI could sit inside Speak Back (for example, give tips after you record).

## 8. Requirements

**P0 (must have for launch)**
1. Send a prompted voice reply (max 60 seconds) to a mutual friend.
2. Receive, play (1× and 0.75×), and reply in a thread.
3. Level-matched prompt library (prompts tied to the learner's course unit).
4. Hints: 3 key phrases + an example answer for each prompt.
5. Report, block, and mute from every message. Feature on/off toggle in settings.
6. Only mutual followers can exchange. No strangers.
7. Age gate: feature hidden for users under the minimum age for each region [ASSUMPTION: confirm with legal].
8. Automated screening of voice (speech-to-text + content filter) before delivery, with a human review queue for reports.
9. "Spoke today" badge on Friend Streak after a completed exchange.
10. Analytics events for all metrics in Section 9.

**P1 (should have, soon after launch)**
1. Push nudge: "Your friend sent you a Speak Back."
2. Speaking history with first vs latest playback.
3. Preset reactions (e.g., "Nice!", "I understood you!", "Say it again?").
4. Auto transcript of the recording, so the listener can read along.
5. Share invite link to bring a friend onto Duolingo.

**P2 (nice to have, later)**
1. AI feedback on your recording (pronunciation tips).
2. Opt-in matching with a stranger at the same level (after safety metrics are healthy).
3. Short live calls with friends.
4. Speak Back inside Friends Quests (e.g., "Trade 3 voice replies this week").

## 9. Success metrics

**North Star metric: Weekly Speaking Learners (WSL)**
- **Definition:** Number of learners who completed at least one full exchange in the last 7 days.
- **Full exchange:** they sent a voice reply **and** received a voice reply in the same thread.
- **Why:** It counts real two-way speaking, not just recording into the void.
- **Calculation:** `count(distinct user_id where sent_voice ≥ 1 AND received_reply ≥ 1 in last 7 days)`
- **Target:** [TARGET - to validate] 5% of eligible users (those with ≥1 mutual friend) within 8 weeks. Reasoning: new opt-in social features usually start small; 5% would be a meaningful but realistic first bar. Revise after the experiment.

**Input metrics (things that drive the North Star)**

| Metric | How calculated | Target |
|---|---|---|
| **1. Send rate** | Users who sent ≥1 voice reply ÷ users who saw the Speak Back entry point, per week | [TARGET - to validate] 15%. Reasoning: first-time speaking to a friend is a big step, so most viewers won't try it. |
| **2. Reply rate within 24h** | Voice replies received within 24h ÷ voice replies sent | [TARGET - to validate] 40%. Reasoning: if most messages go unanswered, the loop breaks and senders give up. |
| **3. Exchanges per speaking learner per week** | Total completed exchanges ÷ WSL | [TARGET - to validate] 2+. Reasoning: one exchange may be curiosity; two or more suggests a habit. |

**Guardrail metrics (must not get worse)**

| Guardrail | How calculated | Threshold |
|---|---|---|
| **1. Daily lesson completion rate** | Users completing ≥1 lesson today ÷ DAU | No statistically significant drop vs control. Speak Back must not replace lessons. |
| **2. Safety: reports per 1,000 exchanges** | (Messages reported ÷ messages sent) × 1,000 | [TARGET - to validate] Below 2. Reasoning: friends-only should be low-risk; a higher rate means the safety design is failing. Pause rollout if crossed. |
| **3. Friend Streak break rate / unfollow rate** | Friend Streaks broken (or unfollows) ÷ active Friend Streaks per week | No significant rise vs control. Pressure to speak must not damage friendships. |

## 10. Experiment plan (A/B test)

**The special challenge:** This is a social feature. If I'm in the test group and my friend is in control, I can't send them anything. That breaks the test. (This is called "network interference.")

**Solution: cluster randomization.** Group users by friend clusters (people connected by mutual follows). Randomly assign whole clusters to test or control.

| Item | Plan |
|---|---|
| **Who is eligible** | Free and paid users, 18+ (or regional minimum age), on mobile, with at least 1 mutual friend, in 3–5 course languages with prompt coverage. |
| **Control group** | Current app. No Speak Back. |
| **Treatment group** | Speak Back (P0 + push nudge). |
| **Split** | 50/50 by friend cluster, starting with a small % of eligible users (e.g., 5%). |
| **Primary metric** | 28-day retention (% of users active on day 28 after entering the test). |
| **Secondary** | North Star (WSL), input metrics, self-reported speaking confidence (in-app 1-question survey at day 21). |
| **Guardrails** | The 3 guardrails from Section 9. |
| **Duration** | At least 4 full weeks. Reasoning: behavior differs by day of week; 28-day retention needs 28 days; and the first week has a "novelty effect" (people try new things just because they're new). |
| **Smallest effect worth detecting (MDE)** | [TARGET - to validate] +1 percentage point in 28-day retention. Reasoning: at Duolingo's scale, even a 1-point gain is many retained users; smaller lifts may not justify the moderation cost. |
| **Sample size** | Use a standard calculator (e.g., Evan Miller's) with: baseline 28-day retention [RESEARCH/ASSUMPTION: unknown — Duolingo doesn't publish it], MDE above, 95% confidence, 80% power. Then **inflate** the number because clusters reduce effective sample size. |

**Main risks to validity**
1. **Spillover:** friends across clusters still talk. Measure how many cross-group friendships exist.
2. **Novelty effect:** early excitement fades. Look at weeks 3–4 separately.
3. **Selection bias:** only people with friends are eligible. Results won't apply to solo users.
4. **Seasonality:** avoid exam season or New Year resolution spikes.
5. **Metric gaming:** people may send silent or 1-second clips. Count a voice reply only if it's ≥5 seconds with detected speech.

## 11. Risks and mitigations

| Risk | Why it matters | Mitigation |
|---|---|---|
| **Safety / harassment** | Voice can carry abuse. HelloTalk users report spam and inappropriate messages [S10]. | Friends-only (mutual follows). 1-tap report and block. Feature off by default for minors (age gate). Clear community rules shown before first send. |
| **Moderation of user voice** | Voice is harder to moderate than text. | Speech-to-text + content filter before delivery. Human review for reported messages. Keep recordings for a limited time [ASSUMPTION: set retention policy with legal]. |
| **Privacy and law** | Voice is personal data. India's DPDP Act 2023 and GDPR apply [UNVERIFIED — check legal specifics]. | Explicit consent. Clear deletion controls. Store minimally. Legal review before launch. |
| **Matching quality** | Friends may be at very different levels or learn different languages. | Prompts adapt to *each* person's level. Show the friend's language. If languages differ, offer "explain in your target language" prompts or suggest same-language friends. |
| **Cold start** (feature needs other people to work) | Users with no friends, or inactive friends, get nothing. | Launch only for users with ≥1 active mutual friend. Invite links (P1). Stranger matching later (P2). |
| **Embarrassment / low use** | Speaking feels risky. Users may never press record. | Hints and example answers. Listen-back before sending. Kind preset reactions. No public scores. |
| **"Events was retired" risk** | Duolingo tried live human sessions before and stopped. | This is async, friends-only, and inside the daily loop, not scheduled. Still a key open question (Section 14). |
| **Hurts core learning** | Users may do Speak Back instead of lessons. | Speak Back doesn't count as the lesson for streaks in v1. Guardrail on lesson completion. |

## 12. Dependencies and rollout plan

**Dependencies**
- Friends graph and Friend Streak service (existing).
- Audio recording, storage and playback infrastructure.
- Speech-to-text for supported languages (for moderation and transcripts).
- Trust & Safety team: rules, review queue, staffing.
- Learning design team: prompt library per course and level.
- Legal / privacy: consent, age gates, retention.
- Notifications team: push nudges.
- Data team: event tracking, cluster randomization.

**Rollout**

| Phase | Who | Gate to move on |
|---|---|---|
| 0. Internal dogfood | Duolingo employees | No major bugs; moderation pipeline works. |
| 1. Fake-door test | Small % of users see a "Speak Back — coming soon" card | Tap rate shows real interest [TARGET - to validate: ≥5% tap rate]. |
| 2. A/B test | 5% of eligible users, 3–5 languages | Primary metric positive; guardrails hold. |
| 3. Gradual expansion | 25% → 50% → 100% of eligible users | Report rate stays under threshold; servers stable. |
| 4. More languages | Remaining courses | Prompt libraries and speech-to-text ready. |

## 13. Roadmap

| **Now** (0–3 months) | **Next** (3–6 months) | **Later** (6–12+ months) |
|---|---|---|
| Research (survey + interviews) | P1: transcripts, speaking history, reactions, invite links | Opt-in stranger matching by level |
| Fake-door test | Speak Back challenges inside Friends Quests | Short live voice calls with friends |
| P0 build + A/B test in 3–5 languages | AI tips on your recording (link to Max upsell) | Group "speaking circles" (only if data supports) |

## 14. Open questions

1. Why exactly was Duolingo Events retired? What lessons apply here? [RESEARCH — verify this]
2. What share of active friendships are in the same language? This decides reach.
3. Should a completed exchange ever count toward the streak itself, or only show a badge?
4. Do users prefer friends, or do they actually want native speakers (like HelloTalk)?
5. How much does voice moderation cost per 1,000 messages at scale?
6. Will this cannibalize Max (Video Call) sign-ups, or help them by building speaking confidence?
7. What's the minimum age by region for voice features?

---

# Part D: Prototype spec (6 screens)

Build these in Figma. Use Duolingo-like style (rounded cards, bright buttons) but **don't copy their logo or characters**. Use your own simple mascot or none.

### Screen 1: Home with Speak Back card
- **Purpose:** Entry point. Show the feature where users already are.
- **Key elements:** Normal learning path in the background. A card above the path: microphone icon, title "Speak Back", text "Practice speaking with Priya today", friend's avatar, Friend Streak flame with day count.
- **Buttons:**
  - `Start` → goes to Screen 2.
  - `✕` (dismiss) → hides the card for today.

### Screen 2: Choose a friend
- **Purpose:** Pick who to speak with.
- **Key elements:** Title "Who do you want to practice with?" List of mutual friends: avatar, name, language flag, level, Friend Streak days. Friends learning a different language are greyed out with "Learning French."
- **Buttons:**
  - Tap a friend row → goes to Screen 3.
  - `Invite a friend` (bottom) → opens share sheet (P1).
  - `←` Back → Screen 1.

### Screen 3: Prompt and hints
- **Purpose:** Reduce fear before speaking.
- **Key elements:** Prompt card in target language with English below, e.g., "¿Qué hiciste el fin de semana? / What did you do at the weekend?" "Helpful words" chips (3). Collapsible "See an example answer." Small text "Your friend will hear this. Be kind."
- **Buttons:**
  - `Shuffle prompt` → loads a new prompt at the same level.
  - `I'm ready` → goes to Screen 4.

### Screen 4: Record and review
- **Purpose:** Record, listen back, send.
- **Key elements:** Big round mic button. Timer "0:00 / 1:00." Live waveform. After recording: playback bar.
- **Buttons:**
  - `Hold to record` (mic) → records while held; release stops.
  - `Play` → plays your recording.
  - `Re-record` → clears and returns to empty state.
  - `Send to Priya` → sends; shows a toast "Sent! We'll tell you when Priya replies." → goes to Screen 5.
- **Rule:** If the clip is under 5 seconds, show "Try saying a little more" and disable Send.

### Screen 5: Conversation thread
- **Purpose:** See the back-and-forth.
- **Key elements:** Thread with the friend. Each message: avatar, prompt label, audio bubble with play button and duration, speed toggle `1×` / `0.75×`, transcript link (P1), reactions row. Banner at top: "You both spoke today 🔥 Friend Streak: 42 days" after a full exchange.
- **Buttons:**
  - `Play` on a bubble → plays audio.
  - `0.75×` → slows playback.
  - Reaction chips `Nice!` / `I understood you!` / `Say it again?` → sends reaction.
  - `Reply with voice` → goes to Screen 4 with the same prompt.
  - `⋯` on a message → opens Screen 6.

### Screen 6: Safety sheet
- **Purpose:** Fast, clear safety controls.
- **Key elements:** Bottom sheet. Short text: "Keep Speak Back friendly and safe."
- **Buttons:**
  - `Report this message` → choose a reason (Inappropriate / Harassment / Spam / Other) → `Submit` → confirmation "Thanks. We'll review this."
  - `Block Priya` → confirm dialog `Block` / `Cancel`. Block hides the thread and stops messages.
  - `Mute Speak Back from Priya` → stops notifications.
  - `Turn off Speak Back` → links to Settings.
  - `Cancel` → closes the sheet.

**Prototype flow to link in Figma:** 1 → 2 → 3 → 4 → 5 → (⋯) 6, plus a "friend replied" notification that opens Screen 5.

---

# Part E: Interview prep

## 8 likely questions with sample answers

**1. "Why this problem? How do you know it's real?"**
"I started with two hypotheses from my own use and from talking to friends. I then designed a survey and interview script to test them. [RESEARCH: Fill in your top finding, e.g., '__ of __ long-time users rated their speaking 1 or 2 out of 5.'] I also checked public data: Duolingo has 135 million monthly users, but only about 9% pay, so most can't use Video Call, its main speaking tool."

**2. "Duolingo already has Video Call with AI. Why build this?"**
"Two reasons. First, Video Call is Max-only, so most users don't have it. Second, AI and friends do different jobs. AI is available anytime and never judges you. A friend gives accountability and a real human voice. Duolingo's own data says Friend Streaks make people 22% more likely to do their lesson. I want to bring that social pull to speaking. The two can work together later, for example AI tips inside Speak Back."

**3. "Why async voice and not live calls?"**
"I scored three options with RICE. Live calls with strangers had the highest potential impact, but low confidence. They have hard problems: matching, time zones, real-time moderation and safety. Async with friends tests the core question cheaply: will people speak to each other at all? If yes, live calls are the next step."

**4. "Duolingo retired Events. Why would this work?"**
"That's my biggest open question, and I don't know the full reason. My design avoids what I suspect were the hard parts: scheduling, strangers, and being separate from the daily loop. Speak Back takes two minutes, works any time, and is inside the Friend Streak. But I'd want to talk to the team that ran Events before building."

**5. "What's your north star, and why not just retention?"**
"Weekly Speaking Learners: people who sent and got a reply in the last 7 days. Retention is the business outcome, and it's my A/B test's primary metric. But it's slow and affected by many things. The north star tells us fast whether the core behavior, two-way speaking, is happening."

**6. "How would you run the A/B test for a social feature?"**
"I can't randomize by user, because a test user's friend may be in control and can't receive messages. So I'd randomize by friend clusters. I'd run at least 4 weeks to measure 28-day retention and see past the novelty effect. Guardrails are lesson completion, report rate and Friend Streak breaks."

**7. "What if the test shows higher engagement but lower lesson completion?"**
"That fails a guardrail, so I wouldn't ship as-is. I'd dig in. Maybe people are swapping a lesson for a voice message. I'd test fixes, like a prompt that unlocks only after the daily lesson. Duolingo's mission is learning, so I wouldn't trade lessons for a new engagement number."

**8. "How would you handle safety?"**
"Start friends-only with mutual follows. 1-tap report and block. Speech-to-text screening before delivery, and human review of reports. Age gates by region. I'd set a report-rate guardrail and pause rollout if it's crossed. Stranger matching only comes after these numbers are healthy for months."

## The 3 weakest points and how to defend them

| Weak point | Why it's weak | How to defend it |
|---|---|---|
| **1. No real data yet** | All evidence slots are empty and all RICE values are my guesses. | "That's why I built the research kit first. The PRD is designed to change based on results. Here's what I'd change if H2 failed: [fill in]." **Best defense: run the survey and interviews before the interview.** |
| **2. Async voice isn't a real conversation** | A 60-second voice note is not the same as a live chat. Critics may say it doesn't solve Problem 1. | "It's a first step that tests willingness to speak to a human, at low risk. Speaking at all is the first barrier. I'd measure self-reported confidence and move to live calls in 'Next' if the data supports it." |
| **3. Reach is limited to users with friends** | Users with no friends on the app get nothing at first. | "Duolingo says 57% of users have at least one friend, so the eligible base is large. Invite links help grow it. Stranger matching is planned once safety is proven. I chose depth with a safe group over breadth with risk." |

---

## Sources

- [S1] Duolingo Blog, "Friend Streak" (5 Aug 2024): https://blog.duolingo.com/friend-streak/
- [S2] Duolingo Blog, "Product lessons from Friend Streak" (20 Sep 2024, updated Feb 2025) — 22% and 57% figures are Duolingo's own claims: https://blog.duolingo.com/product-lessons-friend-streak/
- [S3] Duolingo Blog, "Friends Quests" (2022, updated 2026): https://blog.duolingo.com/friends-quests/
- [S4] Duolingo Investor Relations, "Duolingo Launches AI-Powered Video Call for Android" (16 Jan 2025): https://investors.duolingo.com/news-releases/news-release-details/duolingo-launches-ai-powered-video-call-android
- [S5] Third-party blog on Events retirement (6 Feb 2023) — not an official source, verify this: https://rebeccasdaf.substack.com/p/duolingo-events-retired-but-mine
- [S6] Duolingo Q3 2025 Shareholder Letter, SEC filing (Nov 2025): https://www.sec.gov/Archives/edgar/data/1562088/000162828025049514/q3fy25duolingo9-30x25share.htm
- [S7] Babbel, "Conversation practice / Babbel Speak": https://www.babbel.com/babbel-conversation-practice
- [S8] TechCrunch, "Babbel adds live classes, games and more" (2 Feb 2021): https://techcrunch.com/2021/02/02/language-learning-service-babbel-adds-live-classes-games-and-more/
- [S9] Languatalk, "Speak App Review" (updated Nov 2026) — written by a competitor, treat as opinion: https://languatalk.com/blog/speak-app-review/
- [S10] TalkDrill, "HelloTalk vs Tandem" (2026) — written by a competitor; user counts are self-reported: https://www.talkdrill.com/blog/compare/hellotalk-vs-tandem/
- [S11] Actual Fluency, "HelloTalk Review" (2021, may be outdated): https://actualfluency.com/hellotalk-review

---

## ✅ What I must do myself before this is complete

- [ ] **Verify existing features myself:** open Duolingo and confirm Stories, Leagues, Friend Streak, Friends Quests and Video Call as they look today. Screenshot them.
- [ ] **Find an official source** for why Duolingo Events was retired (or note that none exists).
- [ ] **Try the competitors** for 1–2 days each: Babbel, Speak, HelloTalk (or Tandem). Update the Part B table from your own use.
- [ ] **Run the survey** (Part A1). Aim for 100+ responses.
- [ ] **Do 8–12 interviews** (Part A2). Take notes, get consent.
- [ ] **Analyze** using Part A3. Write a verdict for each hypothesis H1–H4.
- [ ] **Fill every `[RESEARCH]` placeholder** with real numbers in "X of N" form.
- [ ] **Rewrite the personas** from your interview data. Remove `[ASSUMPTION]` only where data supports it.
- [ ] **Revisit RICE scores and targets** using what you learned. Change the chosen option if the data says so, and explain why.
- [ ] **Build the Figma prototype** from Part D. Link all 6 screens. Test it with 3 people.
- [ ] **Add a short "What I learned / what changed" section** at the top. Interviewers love seeing you change your mind based on evidence.
- [ ] **Practice Part E answers out loud**, using your real findings.
- [ ] **Re-check all public numbers** before sharing (they change every quarter).