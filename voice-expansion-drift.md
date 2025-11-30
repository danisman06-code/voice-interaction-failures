Expansion Drift in LLM Voice Interaction

Why the Model Talks Too Much When the User Asks for Very Little



Expansion drift is the systematic tendency of LLMs to produce more content than the user asked for.

In text mode this is mostly an annoyance.

In voice mode it becomes one of the main triggers of cognitive overload, irritation, and session abandonment.



This document analyzes expansion drift specifically in spoken interaction.



1\. Definition



Expansion drift in voice interaction is:



The model’s persistent tendency to answer a narrow question with a broad, over-detailed, multi-layered spoken response.



Key characteristics:



unnecessary elaboration



extra options and scenarios



unsolicited advice and commentary



repeated information



filler transitions (“if you’d like…”, “additionally…”, “it might also help to…”)



Even when the content is factually correct, the quantity and scope are misaligned with the user’s intent.



2\. Why It Is Worse in Voice than in Text

2.1 No skimming



In text, the user can skim or skip.

In voice, the user must listen through or manually interrupt.



2.2 Linear time cost



Every extra sentence consumes real time.

Overlong answers are felt as time theft.



2.3 Cognitive bandwidth



Listening is serial; you cannot easily multitask.

Long monologues increase mental fatigue.



2.4 Friction compounding



Expansion drift combines with:



turn-taking failure



stop-signal failure



rhythm mismatch



to create high-friction experiences very quickly.



3\. Behavioral Patterns



3.1 Narrow question → wide answer

User asks for a single fact; model responds with:



context



background



scenarios



risk analysis



recommendations



3.2 “Helpful” padding

Model includes:



politeness formulas



reassurance phrases



softening language



meta-commentary about what it is doing



3.3 Option explosion

The model lists multiple alternatives when the user implicitly wanted one.



3.4 Prefaced and postfixed content

Intro sentences + outro sentences that add nothing to the requested information.



3.5 Chain reaction with follow-up offers

“Do you want a 5-day forecast?”

“Should I also summarize X?”

These are launched without being asked.



4\. Underlying Mechanism

4.1 Helpful-maximization heuristic



LLMs are trained to:



be thorough



anticipate follow-up questions



reduce the need for another query



In text, this sometimes feels “useful”.

In voice, it feels overbearing.



4.2 Training distribution bias



Most training examples reward:



complete answers



expanded explanations



context plus conclusion



Minimal, single-sentence answers are underrepresented.



4.3 Safety and politeness overlays



RL policies often encourage:



extra disclaimers



hedging



softening



additional context



This adds more tokens to every response.



4.4 Lack of voice-specific compression policy



The model is not explicitly told:



“In voice mode, shorter is better unless the user explicitly asks for depth.”



So it behaves like a text engine with a speaker attached.



5\. Example Scenarios



Example 1 – Weather



User:

“What’s the weather tomorrow in Ankara?”



Text-aligned human answer:

“Partly cloudy, around 10°C.”



Expansion drift voice answer:

“Tomorrow in Ankara it will be partly cloudy, with temperatures around 9 to 10 degrees during the day and cooler at night. You might want to wear a light jacket. If you’d like, I can also give you a 5-day forecast and mention any potential rain or wind changes.”



Example 2 – Simple fact



User:

“What time is it in London right now?”



Human-like answer:

“It’s 3:15 p.m. in London.”



Expansion drift answer:

“Right now it is 3:15 p.m. in London. Keep in mind that London follows UK time, which can shift due to daylight saving changes. If you are planning meetings or travel, I can also help you convert between your local time zone and London time for specific dates.”



6\. Interaction-Level Consequences



Expansion drift in voice mode causes:



longer turns for the model



fewer opportunities for the user to speak



higher cognitive load



increased probability of interruption attempts



more frequent stop-signal failures



accelerated friction buildup



The user starts with a simple intent and ends up:



waiting too long



trying to interrupt



feeling ignored



abandoning voice mode



7\. Interaction with Other Failures



Expansion drift heavily interacts with:



Turn-taking failure

User tries to cut off the overlong answer; model ignores the attempt.



Stop-signal failure

User says “short answer”, “stop”, or “wait”; model continues elaborating.



Rhythm desynchronization

Monologue-style output replaces natural back-and-forth rhythm.



Friction dynamics

Overlong speech directly feeds irritation, impatience, and loss of trust.



Expansion drift is not just a verbosity issue;

it is a structural accelerator of all other voice-mode failures.



8\. Alignment Implications



Mitigating expansion drift requires:



Voice-specific brevity policies

Default to minimal answers unless asked otherwise.



Intent-bounded response generation

Strictly match scope to the user’s question.



Explicit “short answer only” mode

Voice engine that prioritizes brevity and rhythm over completeness.



Anti-padding filters

Remove unnecessary openings, closings, and hedging in voice.



User-controlled depth switches

Commands like “details please” to intentionally expand,

instead of expansion being the default.



Integration with turn-taking and stop-signal systems

Shorter answers create more natural entry points and reduce friction.



9\. Relation to Core Document



This file elaborates on the expansion drift section of:



voice/voice-interaction-core.md



Expansion drift is one of the four central pillars of the voice interaction breakdown cluster, alongside:



turn-taking failure



stop-signal failure



friction dynamics



Together, they explain why seemingly “helpful” voice behavior feels overwhelming and misaligned in real human dialogue.

