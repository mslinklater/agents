# agents

A collection of custom GitHub Copilot coding agents tailored for game development with Unity and C#. These agents live in `.github/agents/` and appear automatically in the Copilot agent picker inside VS Code (1.99+) and on GitHub.com.

## Available Agents

| Agent | File | Description |
|---|---|---|
| **Unity Best Practices** | `unity-best-practices.agent.md` | Reviews and improves Unity C# code for correctness, maintainability, and Unity-specific idioms. Flags anti-patterns, bad lifecycle usage, memory leaks, and naming violations. |
| **Unity Performance Optimiser** | `unity-performance.agent.md` | Analyses Unity projects for CPU, GPU, and memory bottlenecks. Recommends and implements optimisations: batching, pooling, allocation elimination, shader precision, and more. |
| **Unity Debugger** | `unity-debugger.agent.md` | Diagnoses and fixes bugs systematically — NullReferenceExceptions, coroutine failures, physics issues, serialisation problems, and platform-specific breakages. |
| **Unity Game Architect** | `unity-architect.agent.md` | Designs scalable game systems using established Unity patterns: ScriptableObject architecture, state machines, event buses, service locator, object pooling, and scene management. |
| **Unity Shader Author** | `unity-shader.agent.md` | Writes, reviews, and debugs ShaderLab / HLSL shaders for Built-in, URP, and HDRP render pipelines. Covers transparency, SRP Batcher compatibility, and common VFX techniques. |

## How to Use

1. Open Copilot Chat in VS Code or on GitHub.com.
2. Click the agent picker (the `@` button or dropdown next to the prompt field).
3. Select the agent you want — e.g. **Unity Debugger** — and describe your problem.

Each agent has a focused persona and a curated set of tools, so it stays on-topic and gives more reliable answers than the general-purpose Copilot assistant.

## Adding New Agents

1. Create a new `.agent.md` file in `.github/agents/`.
2. Add YAML frontmatter with at least a `description` and a `name`.
3. Write the agent's instructions in the Markdown body.
4. Add a row to the table above.

See the [GitHub Copilot custom agents documentation](https://docs.github.com/en/copilot/how-tos/use-copilot-agents/coding-agent/create-custom-agents) for the full frontmatter reference.
