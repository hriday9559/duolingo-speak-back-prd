# Speak Back — Peer Speaking Practice for Duolingo

An independent product-management portfolio project by Hriday Patel.

> **Portfolio project:** This is an independent concept exercise. It is not affiliated with, endorsed by, or produced by Duolingo.

## The idea

Speak Back explores whether Duolingo learners would benefit from exchanging short, prompted voice replies with mutual friends. The concept connects real-person speaking practice to the existing social habit loop, while avoiding the pressure of live calls or conversations with strangers.

## Project status

**Current source of truth:** [Speak Back — Product Requirements Document v0.4](docs/Speak-Back-PRD-v0.4.md) (25 November 2026).

Version 0.4 is the consolidated main PRD. It brings together the original product requirements, completed survey and interview research, product decisions, prototype walkthrough, UAT findings, metrics, experiment proposal, safety requirements and roadmap. The original v0.3 draft and the dated post-prototype update are retained in `docs/archive/` for historical reference.

## Research and validation

- **Survey:** 55 merged responses; 53 retained after cleaning. The sample comes primarily from the author's network and is directional, not representative.
- **Interviews:** Six interviews conducted in November 2026 (three active and three lapsed learners). Notes are summaries, not verbatim transcripts.
- **Prototype walkthrough:** Three participants tested the six-screen interactive prototype. All three found the core flow understandable; no major usability problems were reported. Some raised safety concerns and some suggested optional AI feedback on individually selected messages.
- **UAT:** Ten checks against the Figma prototype: 8 Pass and 2 Fail. The failures were the missing recording timer/duration validation (UAT-06) and missing preset reactions (UAT-09). UAT-05 and UAT-07 passed for UI flow only.
- **Prototype limitation:** Voice recording and playback are simulated; the Figma prototype does not capture real microphone audio. UAT does not validate real audio capture, playback, upload or moderation.
- Product decisions, personas, RICE scores, targets and experiment assumptions are labelled as assumptions or proposed targets where applicable.

## Key documents

- [Main PRD v0.4](docs/Speak-Back-PRD-v0.4.md) — current consolidated product requirements document
- [UAT test cases and results](docs/UAT-Test-Cases.csv) — 10 prototype checks with actual results
- [User journey map](design/Speak-Back-User-Journey-Map.md) — proposed experience map, user needs and validation opportunities
- `research/` — research appendix, interview synthesis and aggregated survey analysis
- `portfolio/` — portfolio case study in Markdown and PDF
- `docs/archive/` — original v0.3 PRD and dated working notes retained for history

## UAT findings

- **UAT-06 — Fail:** The prototype has no timer or duration indicator, so the five-second minimum cannot be verified.
- **UAT-09 — Fail:** Playback and speed controls work, but preset reaction options are missing from the prototype.
- The UAT results validate the clickable prototype experience only; they do not validate real microphone capture or audio playback.

## Files intentionally kept private

The original timestamped raw survey export and formula-driven analysis workbook are not included in the public repository. This avoids publishing unnecessary respondent-level or timestamp data.

## Evidence and integrity

Report survey findings as counts (for example, “30 of 53”), state the denominator, and disclose sample limitations. Report interview themes as qualitative findings, not population estimates. Describe prototype feedback as early qualitative usability evidence, not proof of demand or retention impact. Do not imply access to Duolingo internal data.

## Author

Hriday Patel

## Portfolio case study

The complete portfolio case study is available in both [PDF format](portfolio/Speak_Back_Case_Study.pdf) and [Markdown format](portfolio/Speak-Back-Case-Study.md). It covers the problem, survey and interview findings, competitive context, product choice, MVP scope, prioritisation, prototype walkthrough, proposed metrics, experiment plan, usability feedback and limitations.

The case study is an independent concept project. The prototype's voice recording is simulated; proposed metrics and experiment targets are not measured outcomes.
