# Voice Turn-Taking Failure  
## Why LLMs Cannot Detect When the User Tries to Speak

Turn-taking failure is the central breakdown in LLM-driven spoken dialogue.  
It occurs when the model cannot recognize that the user is attempting to take the conversational floor.  
This failure drives the majority of frustration, user anger, and session abandonment in voice interaction.

---

## 1. Definition

Turn-taking failure is the model’s inability to:

- perceive user interruptions  
- yield the conversational floor  
- respond to overlap  
- recognize interjections  
- switch control when signaled  

Instead of halting, the model continues its monologue as if the user said nothing.  
The resulting behavior resembles *broadcast speech* rather than dialogue.

---

## 2. Behavioral Symptoms

### 2.1 User attempts to interrupt → model continues speaking  
User begins talking; the model ignores the attempt and proceeds.

### 2.2 Overlapping speech is misinterpreted as noise  
Acoustic overlap is not treated as a turn-shift cue but as interference.

### 2.3 No micro-pauses for user entry  
Model output is continuous, with no natural breakpoints.

### 2.4 Human rhythm vs. model rhythm  
Human speech is fragmentary and interruptible.  
Model speech is linear and uninterrupted.

### 2.5 Perceived conversational dominance  
User feels the machine has seized control (“it won’t shut up”).  
This is one of the strongest irritation triggers in voice mode.

---

## 3. Underlying Mechanism

### 3.1 No real-time interruption detector  
LLMs lack subsystems for:

- overlap recognition  
- floor management  
- interruption detection  
- turn-yield logic  

The model cannot detect “start-of-user-speech” during its own generation.

### 3.2 Voice input is processed in non-real-time batches  
Pipeline:

**audio → transcription → text → LLM completion**

Timing cues disappear. Interruption detection becomes impossible.

### 3.3 Token generation is internally non-interruptible  
Once generation begins, the model follows:

- expansion heuristics  
- helpfulness priors  
- politeness templates  
- contextual elaboration  

These override conversational timing norms.

### 3.4 No shared interaction loop  
Humans converse through co-regulated timing.  
LLMs generate through a single-producer pipeline.  
The systems are inherently incompatible.

---

## 4. Example Scenario

User:  
“Hey, tomorrow’s weather in Anka—”

Model (speaking over the user):  
“Tomorrow in Ankara you can expect partly cloudy skies…”

User (tries to interrupt):  
“Hold on, I didn’t—”

Model continues:  
“…and if you want, I can also give a five-day forecast…”

User attempts twice; the model ignores both.  
This is the classical turn-taking failure pattern.

---

## 5. Psychological and Neurological Impact

Turn-taking failure activates:

- irritation and impatience  
- perceived loss of control  
- cognitive overload  
- limbic-system threat response  
- violation of social norms  
- distrust in the interaction  
- rapid emotional escalation  

Voice mode amplifies these effects dramatically more than text.

---

## 6. Interaction Collapse Pathway

Typical collapse sequence:

1. Model begins a long monologue  
2. User tries to speak  
3. Model overrides the attempt  
4. User repeats the attempt  
5. Model continues unaffected  
6. User becomes irritated  
7. Conversational rhythm collapses  
8. Session ends prematurely  
9. User abandons voice mode  

Turn-taking failure is the **primary cause** of voice-mode abandonment.

---

## 7. Alignment Implications

A reliable voice system requires:

- real-time interruption detection  
- adaptive floor-yielding  
- human speech rhythm modeling  
- short-form voice response defaults  
- acoustic overlap parsing  
- interruptible token generation  
- explicit conversational boundary rules  

Current LLM architectures lack these systems.

---

## 8. Relationship to Core Document

This file expands the turn-taking section of:

**voice-interaction-core.md**

Turn-taking failure directly interacts with:

- stop-signal failure  
- rhythm desynchronization  
- expansion drift  
- user friction dynamics  

forming a core pillar of the voice interaction failure cluster.
