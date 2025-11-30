# Voice Interaction Failure Modes in LLMs

This repository provides a focused analysis of how large language models misalign, drift, and fail during spoken, real-time dialogue. The work maps failure patterns unique to voice mode and highlights timing, rhythm, and structural mismatches between human speech and model-generated responses.

## Core Scope

### Turn-taking breakdowns  
Timing desynchronization, overlap errors, dominance drift, response-window collapse.

### Stop-signal insensitivity  
Failure to stop speaking on cue, delayed termination, override resistance.

### Friction dynamics  
User-agency degradation, grounding instability, cognitive-load escalation.

### Expansion drift  
Unsolicited elaboration, scope growth, runaway suggestion loops.

### Interaction-core failures  
Memory segmentation issues, boundary collapse, multi-turn degradation under spoken load.

## Why Voice Behaves Differently

Voice introduces constraints LLMs are not architecturally optimized for:

- real-time rhythm coupling  
- strict turn-taking boundaries  
- stop-signal compliance  
- microsecond timing expectations  
- pacing symmetry between human and model  

Violating these constraints triggers predictable drift sequences.

## Repository Structure

### voice-index.md  
Master index for all voice-related failure types.

### voice-interaction-core.md  
Structural breakdown of voice-mode memory and boundary behavior.

### voice-turn-taking-failure.md  
Desync, early/late onset, overlap, dominance drift.

### voice-stop-signal-failure.md  
Stop-signal blindness, forced continuation, termination failures.

### voice-friction-analysis.md  
Grounding failures, rhythm instability, user friction dynamics.

### voice-expansion-drift.md  
Expansion loops, unsolicited scope growth, semantic drift.

## Purpose

This work aims to:

- document voice-specific failure modes  
- map drift sequences unique to spoken dialogue  
- clarify why voice alignment is harder than text alignment  
- support research on real-time conversational AI stability  
