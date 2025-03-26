---
title: "Mimicking Human Beings"
date: 2025-03-24 14:30:00 +0100
categories: [AI]
tags: [ai]
image:
  path: /assets/img/posts/mimicking-human-interactions/mimicking-humans.png
  alt: Mimicking Humans
---


### Abstract

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

### The goal

The ultimate goal is to develop an intelligent system that transforms the complex, multi-faceted challenge of travel planning into a streamlined, personalized experience. This system will go beyond basic itinerary creation by integrating various crucial factors that humans naturally consider when planning their journeys.

The system will:

  - Analyze real-time weather patterns and historical climate data
  - Evaluate accommodation options based on personal preferences and past experiences
  - Process and prioritize local recommendations and reviews
  - Learn from users' previous travel experiences and feedback
  - Consider cultural events, seasonal activities, and local customs
  - Factor in budget constraints and value optimization

### Starting the journey

Our starting architecture creates a dynamic interaction where a *demander* form a one-to-one relationship with each *solver*, enabling continuous communication between them.
This back-and-forth exchange allows *solvers* to provide specialized expertise and capabilities while maintaining their independent functions.
The architecture establishes clear boundaries between different *solvers*, ensuring each can focus on their specific responsibilities without interference.
Each *solver* operates with a dedicated purpose, offering unique resources and tools that contribute to the overall system while maintaining their autonomy.

The beauty of this approach is in its simplicity. While the system itself is straightforward, it creates a foundation where each *solver* provides focused functionality in isolation, yet multiple *solvers* can be combined seamlessly through a shared protocol that enables interoperability. Just as primitive structures evolve to meet new needs, our architecture follows design principles where features can be added progressively as *solvers* and *demanders* evolve independently.

In this first release, we are implementing a *demander* - a component that will request a random websites that contains a specific word in the title and it will receive information from *solvers*.

¿Keep with me to see how this solution evolves!


![Architecture](/assets/img/posts/mimicking-human-interactions/mimicking-humans-architecture.png)


Follow all the implementation details yourself using this [github](https://github.com/ramondiez/mimicking-human-beings) repository




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