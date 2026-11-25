> **ARCHIVED NOTE:** This 22 November 2026 post-prototype update has been incorporated into the [consolidated main PRD v0.4](../Speak-Back-PRD-v0.4.md). Keep this file only as a dated record of the initial prototype feedback and AI-feedback proposal.

---

# Speak Back — PRD v0.4 Post-Prototype Update

**Date:** 22 November 2026  
**Author:** Hriday Patel  
**Status:** Portfolio project strategy update; not a complete replacement of the v0.3 full-text PRD.

> Speak Back is an independent product concept and is not affiliated with or endorsed by Duolingo.

## 1. What changed

The project has progressed from survey and interview research into a six-screen interactive prototype. Three participants completed a walkthrough of the prototype. This update records their feedback and the resulting product decisions.

## 2. Prototype usability testing

### Objective
Assess whether learners can understand and navigate the proposed Speak Back flow: Home → Choose Friend → Speaking Prompt → Record and Review → Conversation, with safety controls accessible from the conversation.

### Findings
- **Participants:** 3.
- All three found the core experience understandable.
- No major usability problems were reported.
- Some participants raised safety concerns. These were discussed in relation to safeguards already proposed in the PRD.
- Some participants suggested optional AI analysis of voice messages, with users choosing which individual message AI may examine.

### Limitations
The prototype simulated recording and playback; it did not capture actual microphone audio. The test evaluated comprehension and navigation, not actual speaking behaviour, audio quality, willingness to exchange voice messages, retention impact or product-market fit. With three participants, findings are early qualitative feedback, not statistically representative evidence.

## 3. Product decisions

| Area | Decision |
|---|---|
| Six-screen core flow | Retain the current interaction design based on this initial test |
| Friend selection | Retain |
| Guided speaking prompts | Retain |
| Recording and review | Retain; validate with real audio in a later functional test |
| Safety controls | Retain and make visible, accessible and effective in implementation |
| AI voice analysis | Add as a post-MVP opportunity for further validation |

The absence of major usability issues in this small test is not proof that the design has no usability problems. Further testing with a broader set of learners is still needed.

## 4. Proposed post-MVP feature: User-Controlled AI Voice Feedback

### User need
Some prototype participants expressed interest in receiving AI feedback on voice messages they had sent. They specifically wanted control over which message could be analysed.

### Proposed experience
1. The user opens a voice message they sent.
2. The user selects **Analyse with AI**.
3. The interface explains what will be analysed and how the audio will be processed.
4. The user explicitly confirms permission for that message.
5. AI returns private feedback, potentially covering pronunciation, grammar and sentence construction.
6. The user can review the feedback and decide what to do next.

### Consent and privacy principles
- AI analysis is off by default.
- No automatic analysis of every conversation.
- Permission is explicit and message-specific.
- Explain audio processing and data handling before confirmation.
- Feedback is private by default and is not shared with the conversation partner unless the user chooses to share it.
- Provide clear controls for audio and analysis data consistent with the product's privacy policy.

### Prioritisation
**Proposed priority: P1 / post-MVP exploration.** This is a feature hypothesis generated from early prototype feedback, not a validated requirement. It remains outside the initial MVP.

Before development, validate user demand, desired feedback types, accuracy and usefulness, privacy expectations, technical feasibility and operating costs.

## 5. Safety follow-up

Participants' safety concerns reinforce existing PRD requirements for mutual-friend access, reporting, blocking, moderation and user controls. The discussion during testing clarified the proposed safeguards to participants; it did not validate that the safeguards are sufficient or effective. Safety design and implementation require dedicated review and testing.

## 6. Next validation steps

1. Test the prototype with a broader mix of active and lapsed learners.
2. Ask participants to explain what they believe happens to a voice message when AI analysis is selected.
3. Validate whether users want pronunciation feedback, grammar feedback, sentence-construction feedback or a combination.
4. Test the message-level consent flow before considering AI analysis for development.
5. Evaluate safety controls and moderation expectations.
6. Build and test a functional audio prototype before making claims about recording experience or engagement outcomes.

## 7. Conclusion

Initial prototype testing suggests that the six-screen interaction flow is understandable to the three participants who tested it. Safety remains a product requirement that needs careful implementation and validation. User-controlled AI voice feedback is a promising post-MVP opportunity, but requires further research before prioritisation for development.
