# Speak Back — Current PRD and project status

**Current working direction:** PRD v0.4 strategy update, 22 November 2026. The original full PRD v0.3 text export remains available at `docs/Speak-Back-PRD-v0.3-full-text.md`; v0.4 is maintained as a dated update rather than represented as a fully rewritten replacement.

## Concept
Speak Back proposes short, prompted asynchronous voice replies between mutual Duolingo friends. It aims to connect real-person speaking practice with an existing social habit, without requiring live calls or stranger matching.

## Survey evidence
- 30 of 53 respondents rated their ability to hold a simple two-minute conversation as 1 or 2 out of 5.
- 25 of 51 said they would like to practise with another learner.
- 29 of 51 preferred a friend format, compared with 9 of 51 who selected a stranger format.
- 23 of 51 selected voice-message formats; 15 of 51 selected live-call formats.

The survey combines two Google Forms collected over approximately six months. There were 55 merged responses and 53 retained after cleaning. Respondents came from the author's network; results are directional and not representative of Duolingo's user base.

## Interview research
Six real interviews were conducted in November 2026: three active and three lapsed Duolingo learners. The interviews were approximately 15 minutes each and were documented as notes, not verbatim transcripts. Findings are qualitative and should not be treated as population estimates.

Themes in the notes included difficulty turning learned material into natural speech, preference for asynchronous voice messages over live calls, and differing preferences for practising with friends versus matched learners. One participant specifically valued being able to re-record. Refer to the research appendix and interview synthesis for detail.

## Prototype validation
Three participants tested the six-screen interactive prototype. All three found the core flow understandable; no major usability problems were reported. Some participants raised safety concerns, which were discussed in light of the safeguards proposed in the PRD. Some also suggested optional AI analysis of selected voice messages, with the user choosing which message may be analysed.

This was a small qualitative test of a simulated prototype. Recording and playback were not connected to real microphone audio. The test does not establish demand, actual speaking behaviour, audio quality, retention impact or product-market fit.

## Current product decision
Retain the MVP focus on asynchronous prompted voice messages with mutual friends. Keep live calls and stranger matching outside the MVP. Treat all reach, impact, confidence, effort, target and experiment values as assumptions or proposed targets unless supported by measured evidence.

## New post-MVP opportunity
Explore user-controlled AI voice feedback as a P1/post-MVP hypothesis. Proposed interaction: the user selects a voice message they sent, chooses an explicit “Analyse with AI” action, reviews what will be processed and confirms. Analysis is opt-in and message-specific; feedback is private by default. This is not part of the MVP and requires further demand, quality, privacy, technical-feasibility and cost validation.

## Key repository documents
- `docs/Speak-Back-PRD-v0.3-full-text.md` — original full v0.3 PRD export.
- `docs/PRD-v0.4-post-prototype-update.md` — strategy, usability findings and post-MVP AI proposal.
- `research/Research-Appendix.md` — research status, methods and reporting limitations.
- `research/Research-Appendix-v1-full-text.md` — detailed research appendix.
