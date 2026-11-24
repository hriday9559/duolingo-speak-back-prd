# Speak Back — User Journey Map

**Project:** Speak Back — Peer Speaking Practice for Duolingo  
**Author:** Hriday Patel  
**Artifact:** Proposed experience map  
**Status:** Design hypothesis informed by research and prototype feedback

> This is a proposed, design-led journey map. User goals, thoughts, friction points and opportunities are hypotheses to validate; they are not direct quotations or observed behaviour unless explicitly identified as prototype feedback.

## Scenario

A learner studying Spanish discovers Speak Back, chooses an eligible friend, responds to a guided prompt with a voice message, listens to their friend's reply and decides whether to continue the exchange.

## Journey map

| Stage | 01 — Discover | 02 — Choose friend | 03 — Prepare | 04 — Record & review | 05 — Exchange | 06 — Stay in control |
|---|---|---|---|---|---|---|
| **User action** | Notices Speak Back on the learning path and opens the feature. | Chooses an eligible friend and continues. | Reads the prompt, plays example phrases or chooses another prompt. | Records up to 60 seconds, listens, re-records if needed and sends the voice message. | Checks delivery, plays the friend's reply, changes playback speed and practises again. | Opens safety controls from the conversation, such as report, block, mute or remove access. |
| **User goal** | Understand the feature and feel ready to try speaking. | Practise with someone familiar and willing to participate. | Find something comfortable to say. | Control the recording and feel confident before sharing. | Understand the response and complete a friendly exchange. | Stop an uncomfortable exchange without losing control. |
| **User thought** *(hypothesis)* | “What is this feature, and is it difficult?” | “Would my friend want to practise with me?” | “What can I say with the language I know?” | “Does my recording sound okay?” | “I wonder what my friend will say.” | “Can I manage this interaction if I feel uncomfortable?” |
| **Potential friction** | Feature value or format is unclear. | No eligible friends; unclear access or consent. | Prompt is too difficult or examples are insufficient. | Recording anxiety, unclear microphone state or inability to recover from an error. | Unclear delivery, delayed reply or confusing playback controls. | Safety controls are difficult to find or their consequences are unclear. |
| **Design opportunity** | Explain the format, timing and expected experience. | Make eligibility, speaking access and consent clear. | Offer level-appropriate prompts and useful phrase hints. | Validate permission, active-recording state, retry and send confirmation. | Make pending, failed, sent, unread and completed states understandable. | Make safety controls discoverable and explain the consequences of each action. |

## Path note

Stages 01–05 represent the core exchange. Safety is an optional branch from the conversation, not a required final step.

## Prototype feedback and resulting product opportunities

Three participants completed a walkthrough of the six-screen prototype.

- **Core experience:** All three participants found the core experience understandable. No major usability problems were reported.
- **Safety and control:** Some participants raised safety concerns. The adequacy and effectiveness of proposed safeguards still require dedicated validation.
- **Optional AI feedback:** Some participants suggested optional AI analysis of voice messages, with the user choosing which individual message could be analysed. This remains a post-MVP opportunity, not part of the initial MVP.

### Derived user stories

1. **Guided speaking experience:** As a language learner, I want a clear, guided process for starting a speaking exchange so that I can participate confidently.
2. **Safety and control:** As a learner, I want to feel safe and retain control over my speaking interactions so that I can participate comfortably.
3. **User-controlled AI feedback:** As a language learner, I want to choose an individual voice message for AI analysis so that I can receive feedback while retaining control over my voice data.

## Areas requiring further validation

- Can users easily locate reporting, blocking and muting controls?
- Are the consequences of blocking, reporting or removing access clear?
- Do users understand who can access, replay or retain a voice message?
- What happens after a report, and can users understand whether action has been taken?
- Would learners find message-specific AI feedback useful, and what consent and privacy expectations would they have?

## Evidence and limitations

- Prototype feedback is early qualitative evidence from three participants, not statistically representative research.
- The prototype simulated recording and playback; it did not capture actual microphone audio.
- The journey stages, user goals, thoughts, friction points and design opportunities are design hypotheses, not measured outcomes.
- No individual tester quotes or tester-attributed findings are available in the documented research.

## Source

- [PRD v0.4 — Post-Prototype Update](../docs/PRD-v0.4-post-prototype-update.md)
- [Research Appendix](../research/Research-Appendix-v1-full-text.md)
