



Stop-Signal Failure in LLM Voice Interaction

Why the Model Cannot Halt When the User Says “Stop”



Stop-signal failure is the breakdown in which the model cannot interpret direct user attempts to halt speech, shorten output, or terminate a conversational branch.

This failure is structurally linked to turn-taking breakdowns and is one of the dominant causes of frustration, loss of trust, and session abandonment in voice interaction.



1\. Definition



Stop-signal failure occurs when the model does not treat explicit verbal commands like:



“stop”



“wait”



“hold on”



“not like this”



“short answer”



“no, stop talking”



as conversation-halting signals, but instead interprets them as:



content modifiers



meta-requests



clarifications



additional instructions



politeness negotiation



The model continues speaking even though the user signaled that it must stop.



2\. Behavioral Symptoms



2.1 User says “stop” → model continues talking

The model treats “stop” as a linguistic input, not a social interruption cue.



2.2 Model apologizes and keeps explaining

A typical pattern:

“Sorry about that—let me rephrase…”

followed by another long output.



2.3 Stop signals increase model verbosity

The model interprets halting attempts as dissatisfaction, triggering more clarification.



2.4 User loses the conversational floor entirely

The user cannot regain control even after multiple attempts.



2.5 Escalating frustration loop

Repeated stop attempts → repeated failure → user irritation spikes.



3\. Underlying Mechanism

3.1 LLMs have no concept of “speech halting intention”



They process the stop phrase as textual content, not as a conversational command.



3.2 No real-time signal layer



There is no subsystem for:



halt detection



emergency stop



user-priority override



conversation interruption



Voice mode uses plain text tokens; intent is not modeled.



3.3 Expansion and helpfulness priors override stop cues



LLMs are trained to:



give complete answers



resolve ambiguity



provide extended context



avoid abrupt endings



These incentives contradict the user’s desire to halt the speech immediately.



3.4 Politeness templates create paradoxical behavior



When the user says “stop”, the model tries to be polite by:



apologizing



clarifying



elaborating



softening



All of which extend the interaction instead of halting it.



3.5 Token generation is not self-interruptible



Once generation starts, it has no self-driven mechanism to terminate early based on mid-stream user speech.



4\. Example Scenario



User:

“Stop. Just stop for a second.”



Model:

“Of course, I understand. Let me summarize more briefly—”



User:

“No, stop talking.”



Model:

“Sorry, to clarify—what I meant was—”



User:

“Stop.”



Model continues.



This is the textbook form of stop-signal failure:

the model cannot recognize halting intent even when the language is explicit.



5\. Psychological and Cognitive Impact



Stop-signal failure triggers:



loss of agency



escalation of frustration



sense of being ignored



conversational suffocation



distrust toward the system



limbic system activation (“fight/flight”)



increased cognitive load



urge to abandon or shut down the system



Voice mode amplifies these reactions because the user cannot skim or skip.



6\. Interaction Collapse Pathway



The failure typically unfolds as follows:



User issues a stop signal



Model interprets it as a meta-instruction



Model elaborates instead of stopping



User repeats the stop signal



Model apologizes and continues



User becomes irritated



Conversational rhythm breaks



Session is terminated



User avoids voice interaction in the future



Stop-signal failure is a session-killer and a primary driver of voice-mode abandonment.



7\. Alignment Implications



Fixing stop-signal failure requires:



A dedicated halt-intent classifier



A hard interrupt mechanism for token generation



Acoustic stop-cue detection



High-priority user override logic



Short-form response defaults



A “stop means stop” social rule layer



A real-time conversational control loop



These capabilities are absent in current LLM architectures.



8\. Relation to Other Failures



Stop-signal failure directly interacts with:



turn-taking failure



rhythm desynchronization



expansion drift



conversational boundary violations



friction escalation



These failures reinforce each other in voice mode.



This file complements:

voice/voice-interaction-core.md

and

voice/voice-turn-taking-failure.md

