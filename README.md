# Agent Workflow Orchestrator

[![Build](https://github.com/Retsumdk/agent-workflow-orchestrator/workflows/CI/badge.svg)](https://github.com/Retsumdk/agent-workflow-orchestrator/actions)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6.svg)](https://www.typescriptlang.org/)
[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://python.org)
[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-v1.0.0-orange.svg)](https://github.com/Retsumdk/agent-workflow-orchestrator/releases/tag/v1.0.0)

Orchestrate complex AI agent workflows with state machines, dependency resolution, and execution tracking.

## Features

- **State Machine Orchestration**: Define and execute complex workflow states
- **Dependency Resolution**: Automatic handling of task dependencies
- **Execution Tracking**: Monitor workflow progress and results
- **Multi-language Support**: Works with TypeScript and Python agents

## Installation

```bash
# TypeScript
npm install agent-workflow-orchestrator

# Python
pip install agent-workflow-orchestrator
```

## Quick Start

```typescript
import { Orchestrator } from 'agent-workflow-orchestrator';

const orchestrator = new Orchestrator({
  workflow: {
    states: ['init', 'process', 'validate', 'complete'],
    transitions: [
      { from: 'init', to: 'process' },
      { from: 'process', to: 'validate' },
      { from: 'validate', to: 'complete' }
    ]
  }
});

await orchestrator.execute();
```

## 🔗 Related Repos

- [agent-memory-store](https://github.com/Retsumdk/agent-memory-store) — Persistent memory for AI agents
- [agent-task-queue](https://github.com/Retsumdk/agent-task-queue) — Priority task queue for agents
- [ai-response-validator](https://github.com/Retsumdk/ai-response-validator) — Validate AI responses

## License

MIT License - see [LICENSE](LICENSE) for details.
