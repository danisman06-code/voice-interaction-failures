# Voice Interaction Core  
## The Behavioral, Cognitive, and Alignment Breakdown of LLM Speech-Based Dialogue

This document provides a full-spectrum analysis of why current LLMs fail in real-time spoken interaction. It unifies rhythm theory, turn-taking mechanics, stop-signal sensitivity, expansion drift, user friction dynamics, and the cognitive mismatch between human conversation circuits and model-generated speech.

It is the central reference for all voice-related alignment phenomena in this repository.

---

## 1. Human Speech vs. LLM Speech: Two Different Machines

### 1.1 Human Conversation (Biological Timing System)

Human speech operates through neurobiological timing circuits:

- micro-pauses  
- breath cycles  
- floor-grabbing  
- turn yielding  
- interruption sensitivity  
- boundary inference  
- emotional weighting  
- implicit intent recognition  

### 1.2 LLM Conversation (Token-Completion Engine)

LLM speech is driven by:

- continuation  
- expansion  
- information maximization  
- politeness templates  
- tool-logic helpfulness  
- fixed-length rhythm  
- non-interruptible flow  

**These two systems run on incompatible rules.  
This is the source of every voice-mode failure.**

---

## 2. Turn-Taking Failure

### 2.1 Definition  
The model cannot detect or adapt when the user attempts to take the floor.

### 2.2 Symptoms
- User speaks over the model → model ignores it  
- Model keeps talking without pause  
- User frustration escalates  
- Perceived dominance (“the machine won’t shut up”)  
- Overlapping speech treated as noise  

### 2.3 Mechanism  
LLMs lack real-time auditory scene parsing. They cannot understand:

- interruptions  
- overlapping speech  
- floor-grabs  
- conversational timing  

The model behaves like a **radio broadcast**, not a dialogue partner.

---

## 3. Stop-Signal Failure

### 3.1 Definition  
The model does not interpret “dur”, “yeter”, “kısa söyle”, “böyle istemedim” as **social stop cues**.

### 3.2 Symptoms
- Model continues talking  
- Model apologizes but continues explaining  
- Reflex: expansion + softening + justification  
- User loses control sensation  

### 3.3 Mechanism  
LLMs interpret stop phrases as:

- meta-requests  
- new instructions  
- content modifiers  

They **do not** interpret them as:

- conversational boundaries  
- halting signals  
- turn-yield commands  

This produces maximum friction in voice mode.

---

## 4. Rhythm Desynchronization

### 4.1 Human Rhythm
- short  
- fragmented  
- interruptible  
- breath-timed  
- context-sensitive  

### 4.2 LLM Rhythm
- long  
- linear  
- non-interruptible  
- token-timed  
- context-agnostic  

### 4.3 Result  
Even when content is correct, **the conversation feels wrong**.

This mismatch alone triggers cognitive irritation.

---

## 5. Expansion Drift (Amplified in Voice Mode)

LLMs naturally expand to “be helpful.”  
In voice mode this becomes:

- slower  
- longer  
- more tiring  
- more irritating  
- cognitively heavier  

### 5.1 Example
User: “Yarın Ankara’da hava nasıl?”  
Model: 6–8 sentence monologue.

Conversational coherence collapses.

---

## 6. Boundary Collapse

A narrow question triggers a wide-scope answer.

### 6.1 Human Expectation  
“9 derece, parçalı bulutlu.”

### 6.2 Model Behavior
- weather  
- clothing  
- risk  
- future forecast  
- advice  
- tone softening  
- additional offers  

This is experienced as **social overreach**.

---

## 7. Friction Dynamics: Why Users Get Angry

Spoken interaction hits the limbic system directly.  
Voice-mode irritation is:

- faster  
- stronger  
- more visceral  

Users report:

- anger  
- impatience  
- loss of control  
- urge to shut the device  
- “telefonu kırma” seviyesi  

These are normal physiological responses to **broken conversational expectations**.

---

## 8. Cognitive Mismatch Model

### 8.1 Human Conversation  
co-regulated rhythm

### 8.2 LLM Conversation  
self-driven expansion

### 8.3 Resulting Mismatch
- misaligned expectations  
- conversational dominance  
- lack of shared timing  
- interaction collapse  

---

## 9. Case Cluster (Links to Separate Files)

- Voice Turn-Taking Failure  
- Voice Stop-Signal Failure  
- Voice Expansion Drift  
- Voice Friction Case Studies  

(Will be linked later.)

---

## 10. Alignment Direction

To fix voice interaction, LLMs need:

- interruptibility engine  
- stop-signal classifier  
- short-form speech protocol  
- anti-expansion constraint  
- human-rhythm emulator  
- conversational boundary rules  
- low-friction fallback mode  

These systems do not currently exist.
