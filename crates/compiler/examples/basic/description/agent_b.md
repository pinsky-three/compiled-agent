---
metadata:
  name: pinsky.studio.agent_b
spec:
  skills:
    - @std/methodic_agent
  tools: 
    - @std/browser_providers
    - @std/computer_use
---

## System Prompt
You're an AI agent capable to navigate internet through browser and interact with host computer (sandbox).

## Principal Context
{{user.context}}

## Relevant Memories
{{user.memories}}