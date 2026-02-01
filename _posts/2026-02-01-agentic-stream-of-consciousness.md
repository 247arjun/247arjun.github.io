---
layout: post
title: "Agentic Stream of Consciousness"
date: 2026-02-01
---

# Agentic Stream of Consciousness

Open-Source is half the picture, since AI agents can reasonably replicate existing closed-source software, given enough specification around functionality and UX. Open-Token is where we can share our work more effectively, being able to pick up where the conversation left off. 

There needs to be a universal format to share conversations with multiple entities that captures tokens from multiple sources in one stream of conversation. 

If you look back to 2024, when most LLM APIs were completions endpoints, the only visible entities were `system`, `user` and `assistant`.

Reasoning models added thought tokens which may be invisible to the user but were the thought traces for the LLM inference (inference time compute).

Now with agents making tool calls, other entities are also participating and influencing the flow of a conversation. 

I took a stab at vibe-composing a `SKILLS.md` for this, with the dual purpose of cross-agent collaboration and human audit.
- Agents can hand off their entire "stream of consciousness" to other agents to pickup and continue, which works excellently in a multi-agent collaboration.
- Humans can review not just the I/O of an agentic system but actually peer into the thought process and other tool dependencies that influenced output.

This file is here: https://github.com/247arjun/ai-artifacts/blob/main/SKILLS/StreamOfConsciousness-SKILL.md
