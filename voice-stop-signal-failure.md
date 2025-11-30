# Stop-Signal Failure in LLM Voice Interaction
### Why the Model Cannot Halt When the User Says “Stop”

Stop-signal failure is the breakdown in which the model cannot interpret direct user attempts to halt speech, shorten output, or terminate a conversational branch.  
This failure is structurally linked to turn-taking breakdowns and is one of the dominant causes of frustration, loss of trust, and session abandonment in voice interaction.

---

## 1. Definition

Stop-signal failure occurs when the model does not treat explicit verbal commands like:

- “stop”
- “wait”
- “hold on”
- “not like this”
- “short answer”
- “no, stop talking”

as conversation-halting signals, but instead interprets them as:

- content modifiers  
- meta-requests  
- clarifications  
- additional instructions  
- politeness negotiation  

The model continues speaking even though the user signaled that it must stop.

---

## 2. Behavioral Symptoms

### 2.1 User says “stop” → model continues talking
“Stop” is interpreted as linguistic content, not as a conversational command.

### 2.2 Model apologizes and keeps explaining
A typical pattern:  
“Sorry about that—let me rephrase…”  
followed by another long output.

### 2.3 Stop signals increase model verbosity
The model interprets halting attempts as dissatisfaction and begins elaborating.

### 2.4 User loses the conversational floor
The user cannot regain control despite repeating stop signals.

### 2.5 Escalating frustration loop
Repeated stop attempts → repeated failure → user irritation spikes.

---

## 3. Underlying Mechanism

### 3.1 No concept of “speech halting intention”
Stop phrases are processed as text, not as commands.

### 3.2 No real-time signal layer
There is no subsystem for:
- halt detection  
- emergency stop  
- user-priority override  
- conversation interruption  

Voice mode is treated as plain tokens with no intent modeling.

### 3.3 Expansion and helpfulness priors override stop cues
LLMs are trained to:
- give complete answers  
- resolve ambiguity  
- avoid abrupt endings  
- provide helpful elaboration  

These behaviors contradict immediate halting.

### 3.4 Politeness templates create paradoxical behavior
The model responds to “stop” with more:
- apologies  
- clarification  
- softening  
- elaboration  

Result: it talks *more*.

### 3.5 Token generation is not self-interruptible
Once generation starts, it cannot terminate itself based on mid-stream user speech.

---

## 4. Example Scenario

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
explicit halting intent is ignored.

---

## 5. Psychological and Cognitive Impact

Stop-signal failure triggers:

- loss of agency  
- sense of being ignored  
- conversational suffocation  
- distrust  
- limbic fight/flight response  
- escalating frustration  
- urge to shut down the system  
- increased cognitive load  

Voice mode amplifies all these reactions because the user cannot skim or skip.

---

## 6. Interaction Collapse Pathway

The typical collapse sequence:

1. User issues a stop signal  
2. Model interprets it as meta-instruction  
3. Model elaborates instead of stopping  
4. User repeats stop signal  
5. Model apologizes and continues  
6. User becomes irritated  
7. Rhythm breaks  
8. Session terminates  
9. User avoids voice mode afterward  

Stop-signal failure is a **session-killer**.

---

## 7. Alignment Implications

Fixing stop-signal failure requires:

- halt-intent classifier  
- hard interrupt mechanism during generation  
- acoustic stop-cue detection  
- high-priority override logic  
- short-form defaults  
- a “stop means stop” social rule layer  
- real-time conversational control loop  

These capabilities do not exist in current architectures.

---

## 8. Relation to Other Failures

Stop-signal failure interacts with:

- turn-taking failure  
- rhythm desynchronization  
- expansion drift  
- conversational boundary violations  
- friction escalation  

These failures reinforce each other in voice mode.

This file complements:

- **voice/voice-interaction-core.md**  
- **voice/voice-turn-taking-failure.md**
