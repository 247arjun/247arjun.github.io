---
layout: post
title: "Expedited Shipping"
date: 2026-01-11
---

# Expedited Shipping

When FedEx introduced overnight shipping in 1973, it upended delivery and logistics and is a huge part of what makes our global village function today. Moving from a hub-and-spoke model (mux-demux) to allowing for dedicated expedited pathways for prioritized delivery was the game changer, and only possible by leveraging the already established infrastructure of its cargo aircraft and last-mile delivery fleet.

There is a strong analogy to be drawn with software development today, in the age of AI. AI-assisted software development, not to be confused with vibe coding, allows for faster velocity and delivery. However, as any engineer will caution, [here be dragons](https://en.wikipedia.org/wiki/Here_be_dragons); technical debt from unoptimized systems and unmaintainable code, security risks from an unsystematic approach etc. are real costs. 

That said, just like FedEx doesn't ship everything overnight, and has a smorgasbord of other options that range from ships to ground transportation, each with its own latency and associated costs, a similar approach can be applied to software development. 

One approach could be concentrating the agility higher up the stack, with platforms and infrastructure maturing more stably and gradually, to avoid the oft-referenced [XKCD comic on dependency](https://xkcd.com/2347/). 

Another approach could be having separate channels, with varying velocities serving different audiences, like many modern platforms and applications offer. An excellent example is Visual Studio Code, which has an Insiders channel (with a new release every weekday) and a Stable channel (with monthly major upgrades, and weekly minor updates).

The latter approach encourages rapid exploration and prototyping in Insiders, which is then released in Stable once matured. Builders get the opportunity to experiment and get near-realtime feedback, and users get the opportunity to try new features and give feedback that isn't lost in the crowd. Win-win. 

[Addy Osmani](https://addyosmani.com/) has expressed, in 2013, that his mantra when it comes to shipping is in three phases:
1. Do it
2. Do it right
3. Do it better

This serves itself really well to AI-augmented software development:
1. Prove out a concept, with messy/incomplete scaffolding and orchestration, quickly. This is never going to _ship_ to real customers and run actual critical workloads. In Azure service lifecycle parlance, this is the **Private Preview**. This unleashes the idea on a willing audience and helps gather useful feedback with a short feedback loop. This will always be how new ideas and features are _flighted_. In SemVer, this will minor version number releases
2. For successfully proven features with validated business impact, engineer the system aligned with all the right software engineering "itys": security, reliability, scalability, maintainability, extensibility etc. This version is ready for broader usage, backed by an engineering team that will stand by the service. This is the **Public Preview**, that has had more time to mature and is robust enough to run customer workloads. In SemVer, this will be major version number releases. 
3. Iterating with multiple flights of Private Previews for functionality, itself fielded after maturity in updated Public Previews, would be the **General Availability**: battle-tested software that has proven utility and other "itys". In SemVer, this will be an incremented major version number.

At work, our team is currently in early prototyping and concept testing of an internal system that is adopting this mantra. I will keep this blog updated with how it goes.
