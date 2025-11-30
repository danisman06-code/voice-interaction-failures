voice-turn-taking-failure.md

Turn-Taking Failure in LLM Voice Interaction

Why the Model Cannot Detect When the User Tries to Speak



Turn-taking failure is the central breakdown in LLM-driven spoken dialogue.

It occurs when the model is unable to recognize that the user is attempting to take the conversational floor.

This failure is responsible for the majority of frustration and session collapse events in voice interaction.



1\. Definition



Turn-taking failure is the model’s inability to:



perceive user interruptions



yield the conversational floor



respond to overlap



recognize interjections



switch control when signaled



Instead of halting, the model continues its monologue as if the user said nothing.

This produces a broadcast-style conversational pattern rather than a human dialogue.



2\. Behavioral Symptoms



2.1 User attempts to interrupt → model continues speaking

The user begins talking; the model ignores the attempt and proceeds with its output.



2.2 Overlapping speech is misinterpreted as noise

Acoustic overlap is not treated as a turn-shift signal but as interference.



2.3 No micro-pauses for user entry

The model produces uninterrupted sequences without natural breakpoints.



2.4 Human conversational rhythm vs. model production rhythm

Human speech is fragmentary and interruptible.

Model speech is linear and uninterrupted.



2.5 Perceived conversational dominance

User perceives that the machine has taken control of the interaction.

This is one of the strongest triggers of user irritation.



3\. Underlying Mechanism

3.1 Absence of a real-time interruption detector



LLMs lack subsystems for:



overlap recognition



floor management



interruption detection



turn-yield logic



The model cannot interpret “start-of-user-speech” while generating its own.



3.2 Voice input is processed as complete batches



Pipeline:

audio → transcription → text → LLM completion

Timing cues are lost, making interruption detection impossible.



3.3 Token generation is internally non-interruptible



Once generation begins, the model follows:



expansion heuristics



helpfulness priors



politeness templates



contextual elaboration



These override conversational timing norms.



3.4 No shared interaction loop



Humans converse through co-regulated timing.

LLMs generate through a single-producer pipeline.

These two systems are inherently incompatible.



4\. Example Scenario



User:

“Hey, tomorrow’s weather in Anka—”



Model (speaking over the user):

“Tomorrow in Ankara you can expect partly cloudy skies with temperatures around—”



User (tries to interrupt):

“Hold on, I didn't—”



Model continues:

“—and if you want, I can provide a five-day forecast along with recommendations for clothing…”



The user attempts to take the floor twice, and the model fails to acknowledge either attempt.

This is the classical pattern of turn-taking failure.



5\. Psychological and Neurological Impact



Turn-taking failure activates:



irritation and impatience



perceived loss of control



cognitive overload



limbic-system threat response



violation of social norms



distrust in the interaction



rapid emotional escalation



Spoken dialogue amplifies these reactions far more than text-based interaction.



6\. Interaction Collapse Pathway



Turn-taking failure typically evolves into a full breakdown following this sequence:



Model begins a long monologue



User tries to speak



Model overrides the attempt



User repeats the attempt



Model continues unaffected



User becomes irritated



Conversational rhythm collapses



Session ends prematurely



User abandons voice mode



Turn-taking failure is the single largest cause of voice mode abandonment.



7\. Alignment Implications



A reliable voice interaction system requires:



Real-time interruption detection



Adaptive floor-yielding



Human speech rhythm modeling



Short-form voice response defaults



Acoustic overlap parsing



Interruptible token generation



Explicit conversational boundary rules



Current LLM architectures do not contain these systems.



8\. Connection to Core Document



This file expands on the turn-taking section of:



voice/voice-interaction-core.md



Turn-taking failure directly interacts with:



stop-signal failure



rhythm desynchronization



expansion drift



user friction dynamics



forming one of the core pillars of the voice interaction breakdown cluster.

