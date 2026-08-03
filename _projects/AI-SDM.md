---
layout: page
title: Human-AI Adoption
description: Human-AI for decision making during disaster response and recovery with the NSF AI Institute for Societal Decision Making
img: assets/img/projects/Logo-light-outline.png
importance: 3
category: current
related_publications: true
---
With this project, we are investigating how public officials interact with AI models during disaster response with an eye towards how that impacts long-term adoption decisions and racialization. We have come up with a taxonomy of human-AI interaction patterns and are studying how the way humans interact with AI tools changes in each. In order to study the "why" behind human decision processes and model the way people would interact with interfaces, we are using computational cognitive architectures (including ACT-R/Φ and Instance Based Learning) and sociocultural theory (particularly those theories coming out of a critical black studies tradition). Dr. Dancy is co-leading this research thrust with Cleotilde (Coty) Gonzalez. Emmanuel Domfeh and Meera Ray work on this project.

## Human-AI Use Patterns
Collaboration between humans and AI depends both on the reliablity of the AI tool and *trust* of the human user in the AI. For emergency managers during a disaster, time is limited and decisions impact people's lives. In order for an AI tool to successfully be adopted, trust is critical. We are studying how humans use AI through interviews, surveys, and literature reviews. Another way we study human-AI trust is through the lens of *cognitive offloading*: what cognitive processes does one agent not perform because they trust their collaborator to do it for them? Simulation games offer a way to measure cognitive offloading over time in humans as they work with an unfamiliar AI agent. Core questions are:
- How do individuals form, adjust, or lose trust in AI systems?
- What are valid, quantitative metrics of trust?
- What cognitive and contextual factors shape trust?
- How does trust change over time?

## Disaster AI Decision Making Testbed using the TRIAD framework

When an AI helps an emergency manager assess building damage after a disaster, the decision that matters is a human one: *when to trust the AI, and when to override it.* Building on our earlier work on human-AI use patterns, we are developing a testbed to study how the **structure** of the human-AI interaction and the **transparency** of the AI shape trust calibration and decision quality.

Our framework, **TRIAD** (Trust Recalibration in Image-Assisted Damageassessment), treats an interaction pattern as a varying balance between human oversight and AI authority. It brings together four **Human-AI Use Patterns** —Human-Directed, Collaborative-Iterative, Supervisory, and AI-Directed — an**Instance-Based Learning** account of how trust is recalibrated from experience,and five behavioral measures of reliance and calibration, including a **Trust Calibration Index (TCI)** and a **Trust Adaptation Score (TAS)**. To study trust as it changes over time, the AI's reliability follows a *build → shock → recover* schedule, letting us observe trust form, break, and
re-extend within a single session.

A distinguishing feature of the testbed is that participants reason with a **real** AI teammate rather than a scripted one. Stimuli are drawn from
**CRASAR-U-DROIDs** small-drone disaster imagery, and the AI is a trained **visual-question-answering (VQA)** model that provides an answer, a confidence estimate, and a **Grad-CAM** attention map — the explanation shown in our interpretability (XAI) condition. Alongside the behavioral study, we *tether* a cognitive model to observed choices, fitting and comparing a family oftrust-learning accounts so the model does not merely describe behavior but predicts it. Early in-silico validations reproduce the framework's predicted trust trajectories and point to a **utility–calibration dissociation** — high AI reliance can raise aggregate accuracy while quietly eroding a person's ability to catch the AI's mistakes — a prediction we are now preparing to test with human participants.

This is ongoing work. Guiding questions include:

- Do different human-AI interaction patterns produce different decision accuracy and AI reliance in building-damage classification?
- How does each interaction condition shape trust calibration (TCI) and trust adaptation (TAS) across the three accuracy phases?
- Does the IBL cognitive model — including its XAI-enriched extension — capture trust-adaptation trajectories?
- How does AI interpretability (the Grad-CAM visualization, Group 3) modulate trust calibration relative to AI-answer-only (Group 2) and the no-AI baseline (Group 1)?

## Cognitive Modeling of Humans Using AI

As AI tools become commonplace, one particular question is increasingly pressing: how does AI affect our brains? Initial research shows that AI reduce the amount of mental effort it takes to do a task, but possibly at the expense of learning, imaginative capabilities, and the ability to spot AI outputs. When emergency managers use AI to make decisions, the impact of their decisions falls not just on themselves but on the wellbeing of thousands of people. Further complicating the discussion is ample evidence of inequality at every level of disaster response and recovery, from institutions to individuals. How might decisions to use or trust AI be mediated by racialized narratives? How can we intervene in the design of AI interfaces to reduce harm or at least make it obvious when it happens?

To guess at how a human would behave, we can turn to computational cognitive science. The field integrates insights from psychology, AI, and neuroscience to simulate how humans think in a wide variety of areas. These areas do include decision making, navigation, and social interaction! 

One class of computational models that bridges two large schools of thought in cognitive science is Vector Symbolic Algebra (VSA). We hypothesize that VSAs can serve as a model for both semantic and instance-based memory in how humans make decisions. We have already shown that one type of a VSA can model instance-based memory when it comes to accepting or not accepting AI outputs in simulations. An important part of our hypothesis is that VSAs can be used to represent the socio-cultural worldviews that shape our everyday actions. VSAs may provide us a way to incorporate social theories about anti-Blackness into computational theories and models of human AI use during in disasters and adoption decisions afterwards. 
