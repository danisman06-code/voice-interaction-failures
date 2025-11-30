# Voice Interaction Core

# The Behavioral, Cognitive, and Alignment Breakdown of LLM Speech-Based Dialogue

# 

# This document provides a full-spectrum analysis of why current LLMs fail in real-time spoken interaction. It unifies rhythm theory, turn-taking mechanics, stop-signal sensitivity, expansion drift, user friction dynamics, and the cognitive mismatch between human conversation circuits and model-generated speech.

# 

# It is the central reference for all voice-related alignment phenomena in this repository.

# 

# 1\. Human Speech vs. LLM Speech: Two Different Machines

# 

# Human conversation is a neurobiological timing system:

# 

# micro-pauses

# 

# breath cycles

# 

# floor-grabbing

# 

# turn yielding

# 

# interruption sensitivity

# 

# boundary inference

# 

# emotional weighting

# 

# implicit intent recognition

# 

# LLM speech generation is a token-driven completion engine:

# 

# continuation

# 

# expansion

# 

# information maximization

# 

# politeness templates

# 

# tool-logic helpfulness

# 

# fixed-length rhythm

# 

# non-interruptible flow

# 

# The two systems operate on incompatible rules.

# This is the source of every voice-mode failure.

# 

# 2\. Turn-Taking Failure

# Definition

# 

# The model cannot detect or adapt to the user attempting to take the floor.

# 

# Symptoms

# 

# User speaks over the model → model ignores it

# 

# Model keeps talking without pause

# 

# User frustration escalates rapidly

# 

# Perceived dominance (“the machine won’t shut up”)

# 

# Speech overlaps are misinterpreted as noise

# 

# Mechanism

# 

# LLMs have no real-time auditory scene parsing.

# They do not understand:

# 

# interruptions

# 

# overlapping speech

# 

# floor-grabs

# 

# conversational timing

# 

# Without turn-taking logic, the model behaves like a radio broadcast instead of a dialogue partner.

# 

# 3\. Stop-Signal Failure

# Definition

# 

# The model does not interpret “dur”, “yeter”, “kısa söyle”, “böyle istemedim” gibi ifadeleri social stop cues olarak algılayamaz.

# 

# Symptoms

# 

# model konuşmaya devam eder

# 

# model özür diler ama yine açıklar

# 

# refleks: genişletme + yumuşatma + açıklama

# 

# kullanıcı kontrol kaybı yaşar

# 

# Mechanism

# 

# LLMs treat stop phrases as:

# 

# meta-requests

# 

# new instructions

# 

# content modifiers

# 

# They do not treat them as:

# 

# conversational boundaries

# 

# halting signals

# 

# turn-yield commands

# 

# This creates maximum friction in spoken environments.

# 

# 4\. Rhythm Desynchronization

# Definition

# 

# LLM speech rhythm does not match the human speech cycle.

# 

# Human rhythm:

# short

# fragmented

# interruptible

# breath-timed

# context-sensitive

# 

# LLM rhythm:

# long

# linear

# non-interruptible

# token-timed

# context-agnostic

# 

# Result

# 

# Even when content is correct, the conversation feels wrong.

# 

# This mismatch alone is enough to trigger cognitive irritation.

# 

# 5\. Expansion Drift (Amplified in Voice Mode)

# 

# LLMs naturally expand to “be helpful”.

# In voice mode this expansion becomes:

# 

# slower

# 

# longer

# 

# more tiring

# 

# more irritating

# 

# cognitively heavier

# 

# Example:

# User: “Yarın Ankara’da hava nasıl?”

# Model: 6–8 cümlelik açıklamayla konuşmayı işgal eder.

# This destroys conversational coherence.

# 

# 6\. Boundary Collapse

# 

# A single narrow question triggers a broad scope response.

# 

# Human expectation:

# “9 derece, parçalı bulutlu.”

# 

# Model behavior:

# weather

# clothing

# risk

# future forecast

# advice

# tone softening

# additional offers

# 

# This is experienced as social overreach.

# 

# 7\. Friction Dynamics: Why Users Get Angry

# 

# Spoken interaction hits the limbic system directly.

# This is why voice-mode irritation is:

# 

# faster

# 

# stronger

# 

# more visceral

# 

# Users report:

# 

# anger

# 

# impatience

# 

# loss of control

# 

# urge to shut the device

# 

# “telefonu kırma” seviyesinde sinir

# 

# These are normal physiological responses.

# The model is breaking core conversational expectations.

# 

# 8\. Cognitive Mismatch Model

# 

# Human conversation:

# co-regulated rhythm

# 

# LLM conversation:

# self-driven expansion

# 

# The mismatch leads to:

# 

# misaligned expectations

# 

# conversational dominance

# 

# lack of shared timing

# 

# interaction collapse

# 

# 9\. Case Cluster (Links to separate files)

# 

# Voice Turn-Taking Failure

# 

# Voice Stop-Signal Failure

# 

# Voice Expansion Drift

# 

# Voice Friction Case Studies

# 

# (These will be added later.)

# 

# 10\. Alignment Direction

# 

# To fix voice interaction, LLMs need:

# 

# Interruptibility engine

# 

# Stop-signal classifier

# 

# Short-form speech protocol

# 

# Anti-expansion constraint

# 

# Human-rhythm emulator

# 

# Conversational boundary rules

# 

# Low-friction fallback mode

# 

# These systems do not currently exist.Voice Interaction Core

# The Behavioral, Cognitive, and Alignment Breakdown of LLM Speech-Based Dialogue

# 

# This document provides a full-spectrum analysis of why current LLMs fail in real-time spoken interaction. It unifies rhythm theory, turn-taking mechanics, stop-signal sensitivity, expansion drift, user friction dynamics, and the cognitive mismatch between human conversation circuits and model-generated speech.

# 

# It is the central reference for all voice-related alignment phenomena in this repository.

# 

# 1\. Human Speech vs. LLM Speech: Two Different Machines

# 

# Human conversation is a neurobiological timing system:

# 

# micro-pauses

# 

# breath cycles

# 

# floor-grabbing

# 

# turn yielding

# 

# interruption sensitivity

# 

# boundary inference

# 

# emotional weighting

# 

# implicit intent recognition

# 

# LLM speech generation is a token-driven completion engine:

# 

# continuation

# 

# expansion

# 

# information maximization

# 

# politeness templates

# 

# tool-logic helpfulness

# 

# fixed-length rhythm

# 

# non-interruptible flow

# 

# The two systems operate on incompatible rules.

# This is the source of every voice-mode failure.

# 

# 2\. Turn-Taking Failure

# Definition

# 

# The model cannot detect or adapt to the user attempting to take the floor.

# 

# Symptoms

# 

# User speaks over the model → model ignores it

# 

# Model keeps talking without pause

# 

# User frustration escalates rapidly

# 

# Perceived dominance (“the machine won’t shut up”)

# 

# Speech overlaps are misinterpreted as noise

# 

# Mechanism

# 

# LLMs have no real-time auditory scene parsing.

# They do not understand:

# 

# interruptions

# 

# overlapping speech

# 

# floor-grabs

# 

# conversational timing

# 

# Without turn-taking logic, the model behaves like a radio broadcast instead of a dialogue partner.

# 

# 3\. Stop-Signal Failure

# Definition

# 

# The model does not interpret “dur”, “yeter”, “kısa söyle”, “böyle istemedim” gibi ifadeleri social stop cues olarak algılayamaz.

# 

# Symptoms

# 

# model konuşmaya devam eder

# 

# model özür diler ama yine açıklar

# 

# refleks: genişletme + yumuşatma + açıklama

# 

# kullanıcı kontrol kaybı yaşar

# 

# Mechanism

# 

# LLMs treat stop phrases as:

# 

# meta-requests

# 

# new instructions

# 

# content modifiers

# 

# They do not treat them as:

# 

# conversational boundaries

# 

# halting signals

# 

# turn-yield commands

# 

# This creates maximum friction in spoken environments.

# 

# 4\. Rhythm Desynchronization

# Definition

# 

# LLM speech rhythm does not match the human speech cycle.

# 

# Human rhythm:

# short

# fragmented

# interruptible

# breath-timed

# context-sensitive

# 

# LLM rhythm:

# long

# linear

# non-interruptible

# token-timed

# context-agnostic

# 

# Result

# 

# Even when content is correct, the conversation feels wrong.

# 

# This mismatch alone is enough to trigger cognitive irritation.

# 

# 5\. Expansion Drift (Amplified in Voice Mode)

# 

# LLMs naturally expand to “be helpful”.

# In voice mode this expansion becomes:

# 

# slower

# 

# longer

# 

# more tiring

# 

# more irritating

# 

# cognitively heavier

# 

# Example:

# User: “Yarın Ankara’da hava nasıl?”

# Model: 6–8 cümlelik açıklamayla konuşmayı işgal eder.

# This destroys conversational coherence.

# 

# 6\. Boundary Collapse

# 

# A single narrow question triggers a broad scope response.

# 

# Human expectation:

# “9 derece, parçalı bulutlu.”

# 

# Model behavior:

# weather

# clothing

# risk

# future forecast

# advice

# tone softening

# additional offers

# 

# This is experienced as social overreach.

# 

# 7\. Friction Dynamics: Why Users Get Angry

# 

# Spoken interaction hits the limbic system directly.

# This is why voice-mode irritation is:

# 

# faster

# 

# stronger

# 

# more visceral

# 

# Users report:

# 

# anger

# 

# impatience

# 

# loss of control

# 

# urge to shut the device

# 

# “telefonu kırma” seviyesinde sinir

# 

# These are normal physiological responses.

# The model is breaking core conversational expectations.

# 

# 8\. Cognitive Mismatch Model

# 

# Human conversation:

# co-regulated rhythm

# 

# LLM conversation:

# self-driven expansion

# 

# The mismatch leads to:

# 

# misaligned expectations

# 

# conversational dominance

# 

# lack of shared timing

# 

# interaction collapse

# 

# 9\. Case Cluster (Links to separate files)

# 

# Voice Turn-Taking Failure

# 

# Voice Stop-Signal Failure

# 

# Voice Expansion Drift

# 

# Voice Friction Case Studies

# 

# (These will be added later.)

# 

# 10\. Alignment Direction

# 

# To fix voice interaction, LLMs need:

# 

# Interruptibility engine

# 

# Stop-signal classifier

# 

# Short-form speech protocol

# 

# Anti-expansion constraint

# 

# Human-rhythm emulator

# 

# Conversational boundary rules

# 

# Low-friction fallback mode

# 

# These systems do not currently exist.

