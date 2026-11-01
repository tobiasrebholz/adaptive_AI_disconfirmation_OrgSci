# Adaptive AI-Assisted Disconfirmation

A reusable experimental infrastructure implemented in Qualtrics for studying reciprocal judgment updating during open-ended human–AI conversations.

## Repository contents

- **Qualtrics code for Experiments 1 and 2**, documenting the survey and parallel ranking and chat implementation.
- **System prompts** governing hidden recommendation updating, substantive stance, interpersonal tone, and fixed or adaptive persistence.
- **Access to the interactive prototype** through the demo link below.

These materials document the existing implementation and provide a starting point for adapting the experimental infrastructure to other structured judgment tasks.

## Interactive demo

▶️▶️▶️ **[Launch the Qualtrics demo](https://duke.qualtrics.com/jfe/form/SV_6gJYJSl6u1RUDWe)** ◀️◀️◀️<br>
[*Ctrl+click* (Windows) or *⌘+click* (Mac) to open in a new tab]

This shortened survey demonstrates the infrastructure using the Mars survival task from Experiments 1 and 2. On the first page, you can select treatment conditions to explore the AI assistant’s different interaction policies. Then, you will be asked to choose a survival strategy and rank a set of 15 salvaged items with chat-based support from an AI assistant.

The demo also includes instructions for inspecting the AI assistant’s hidden reasoning traces alongside the visible conversation.

## How the experimental infrastructure works

The infrastructure combines three components:

1. **Repeated structured judgments.** Participants can revise their item rankings throughout the conversation, providing a process measure of judgment updating.

2. **Parallel hidden reasoning traces.** Before each visible reply, the assistant generates its current recommended strategy and item ranking in a separate, non-user-facing reasoning trace. Under adaptive persistence, it also estimates the likelihood that the user will accept its opposing strategy.

3. **Experimentally controlled interaction policies.** System prompts govern substantive agreement or disagreement, interpersonal tone, and persistence. Fixed persistence uses conversational turn counts to govern when concession becomes permissible; adaptive persistence uses thresholds applied to the assistant’s persuasion probability estimates.

Pairing participants’ evolving judgments with the assistant’s elicited recommendations makes it possible to distinguish user updating, AI accommodation, and movement by both parties. Researchers can investigate these trajectories without first reconstructing task positions from conversational traces.

# LICENSE

Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
