---
title: "Mimicking Human Beings"
date: 2025-03-24 14:30:00 +0100
categories: [AI]
tags: [ai]
image:
  path: /assets/img/posts/mimicking-human-interactions/mimicking-humans.png
  alt: Mimicking Humans
---

## Mimicking Human Interactions

Welcome to my blog series where we'll explore how to build an agentic solution that mimics human daily interactions. In this series, we'll examine how complex human behaviors can emerge from simple rules of interaction between agents.
Each chapter will introduce a concept or feeling and I will provide its implementation, showing how agent-based models can represent human-like interactions while maintaining simplicity at their core.

Agent-based thinking, views social interactions as occurring when both parties prefer having them over not having them, with each seeking the form of interaction that ranks highest in their preferences.
This approach isn't limited to monetary exchanges between strangers but extends to scientific collaborations, romantic relationships, and commitments to voluntary organizations - all captured by the same logical framework.

As we progress through this series, we'll explore how agents can be designed with varying degrees of human-likeness, carefully selecting which features to faithfully match and which to deliberately omit.
We'll examine how people naturally attempt to "naturalize" unfamiliar agents by integrating them into their existing frameworks of knowledge and expectations.
This process of accommodation and adaptation reveals how humans test boundaries of commonly shared expectations to assign new entities a place within their familiar cognitive and practical order.

By understanding these dynamics, we can create agent-based models composed of decision-making heuristics, non-linear interaction topologies, and learning rules that generate complex emergent behaviors from simple foundations.

Join us as we decode the fascinating intersection of human behavior and artificial agency!

### Journey Kick Off

In the world of complex systems, interactions between agents follow simple rules that lead to emergent behaviors and structures.
Agent-based modeling represents a bottom-up approach where the richness of structures comes from these simple interaction rules.
This approach allows us to simulate how micro-level interactions lead to the emergence of structure and organization at the macro level.

When we begin with basic interactions, we focus on featureless agents interacting with each other.
These agents can be programmed to follow specific rules that guide their behavior, similar to how birds in a flock follow three simple rules: separation (avoiding crowding), alignment (steering toward average heading), and cohesion (moving toward average position).
Through these simple local interactions, complex global patterns emerge.

As our solution evolves, we can enhance these basic agents by giving them internal states where they can store energy and information.
Some advanced models don't require all agents to interact directly or have complete information about the system.
Instead, they operate based on local information and short-term behavior, similar to how humans make decisions with limited information.

The beauty of this approach is that many previously intractable problems suddenly become accessible.
By focusing on the interactional structure rather than the complexity of each individual agent, we can model various systems - from neurons in a brain to humans in a market - all understood as systems of interacting agents.
This mimics how real-world social interactions occur, where both parties engage when it benefits them and seek interactions that align with their preferences.

### Technology Stackset

The initial solution is based on an open-source framework called [Model Context Protocol](https://modelcontextprotocol.io/introduction) (MCP). MCP includes three fundamental primitives that enable rich interactions between clients, servers, and language models:

  - Prompts: These are pre-defined templates or instructions that guide language model interactions and are user-controlled through slash commands or menu options.

  - Resources: These provide structured data or contextual content to the model and are application-controlled, including file contents or git history.

  - Tools: These are executable functions that allow models to perform actions or retrieve information, such as API requests or file writing, and are model-controlled.

The MCP Server implements the server-side of the protocol, responsible for exposing tools, managing resources, providing prompt templates, supporting capability negotiation, implementing.

#### Benefits

- MCP functions like a USB-C port (*it has taken a while*) for AI applications, providing a standardized way to connect AI models to various data sources and tools.
- MCP standardization helps applications provide context to LLMs through an open protocol. 
- MCP provides a growing list of pre-built integrations that LLMs can directly plug into.




### Inial Approach

Our starting architecture works like this: we have a client that sends requests, and servers that respond with information.
This back-and-forth creates a conversation where one part asks and another answers, much like how we naturally interact with our environment to get what we need.

The beauty of this approach is in its simplicity. While the system itself is straightforward, it creates a foundation that can grow more complex over time.
Just as primitive structures evolve to meet new needs, our architecture will develop additional components as we move forward.

This interaction mimics how living things process information from their surroundings. Everything is present in the original, simple forms - a basic unit interacting with its environment, taking in what it needs.
Our system follows this natural pattern, where the apparent complexity of behavior reflects the environment it operates in.

As we continue building, we'll add more agents and components to handle increasingly complex interactions.
This gradual evolution mirrors how simple local exchanges can eventually lead to more sophisticated systems and behaviors.


![Architecture](/assets/img/posts/mimicking-human-interactions/mimicking-humans-architecture.png)


Follow all the implementation details yourself using this [github](https://www.google.com) repository !!!