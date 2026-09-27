# GenPark Autonomous Personal Delegator Skill

[![GenPark Certified](https://img.shields.io/badge/GenPark-Certified%20Skill-00E599?style=flat-square)](https://genpark.ai)
[![Protocol](https://img.shields.io/badge/MCP-Standard%20Skill-6A0DAD?style=flat-square)](https://genpark.ai)
[![Category](https://img.shields.io/badge/Category-Service%20Agent-blue?style=flat-square)](https://genpark.ai)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=flat-square)](LICENSE)

> GenPark AI Agent Skill - Autonomous micro-action delegation with user guardrails, confidence thresholding, dry-run previews, and token budget gating.  
> *Inspired by architectural paradigms from Instinct (instinct.is).*

---

## 🌟 Overview & Architecture

Modern personal agents must evolve past static prompt-response turn-taking into **continuous ambient cognitive companions**.  
The `genpark-autonomous-personal-delegator-skill` brings production-grade primitives for Model Context Protocol (MCP) clients, autonomous agent swarms, and personal assistants operating within the GenPark ecosystem.

```
+-------------------------------------------------------------+
|                GenPark Personal Agent Swarm                 |
+-------------------------------------------------------------+
       |                                              |
       v                                              v
+-----------------------------+        +------------------------------+
|   Zero-Prompt Anticipator   |        |   Hierarchical Memory Stream |
| (Activity & Context Sensing)|        |   (Temporal Decay & Vectors) |
+-----------------------------+        +------------------------------+
       |                                              |
       +----------------------+-----------------------+
                              |
                              v
       +----------------------------------------------+
       |     Autonomous Guardrailed Micro-Delegator    |
       |  (Sandboxed Dispatch & Token Budget Gating)  |
       +----------------------------------------------+
```

---

## 🛠️ Exposed Tools & Capabilities

### `evaluate_delegation_safety`
Scores proposed autonomous actions against user risk boundaries, reversible impact levels, and required permissions.

### `stage_micro_action`
Stages non-destructive micro-actions in a dry-run state awaiting automatic or single-click confirmation.

### `execute_sandboxed_dispatch`
Executes verified micro-actions across connected agent tools within strict token and latency budgets.


---

## 🚀 Quickstart & MCP Configuration

Add this skill to your `genpark.config.json` or Claude / Cursor desktop MCP configurations:

```json
{
  "mcpServers": {
    "genpark-autonomous-personal-delegator-skill": {
      "command": "npx",
      "args": ["-y", "@alphapark/genpark-autonomous-personal-delegator-skill"],
      "env": {
        "GENPARK_API_KEY": "your_genpark_api_key"
      }
    }
  }
}
```

---

## 📄 License
Apache-2.0 © 2026 GenPark AI Inc. (alphaparkinc)
