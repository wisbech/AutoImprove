# AutoImprove

A revolutionary framework for autonomous, recursive AI-driven project development using pure markdown and folder structures.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## What is AutoImprove?

AutoImprove transforms any project into a self-improving, agent-navigable workflow. Inspired by Jake van der Plas's folder structure system and Karpathy's autoresearch, it enables AI agents to autonomously evaluate progress, spawn sub-tasks, and iterate toward goals—all through readable markdown files.

### Key Features
- **Pure Markdown**: No code required—works with any AI agent/editor (Claude, opencode, pi, goose, openclaw, etc.).
- **Recursive Agent System**: Each workspace has its own `AUTOIMPROVE.md` with metrics, rules, and logs for deep nesting.
- **Routing Table Navigation**: Agents use tables to seamlessly move between tasks and workspaces.
- **Self-Improving**: Built-in evaluation levers (metrics, children, rules, logs) for autonomous iteration.
- **Generic and Adaptable**: Drop into any project—software, research, content, business—and instantly enable AI-driven improvement.
- **No Lock-In**: Decoupled from specific tools; agents read and edit markdown directly.

## How It Works

1. **Root AUTOIMPROVE.md**: Project overview, routing table, metrics, rules, and logs.
2. **Workspace AUTOIMPROVE.md**: Task-specific details, sub-routing, local metrics/rules.
3. **Agent Autonomy**: Agents evaluate conditions, spawn sub-workspaces, update progress, and log actions.

### Core Components
- **Routing Table**: Matches tasks to workspaces/files.
- **Metrics**: Track progress against targets.
- **Children**: Sub-workspaces with weights/status.
- **Rules**: Condition-action pairs for automation.
- **Logs**: History of actions and results.

## Quick Start

1. Copy `AUTOIMPROVE_TEMPLATE.md` to your project root as `AUTOIMPROVE.md`.
2. Customize:
   - Project overview and goals.
   - Routing table for your workspaces.
   - Metrics, rules, and logs.
3. Create workspace folders (e.g., `research/`, `implement/`) with their own `AUTOIMPROVE.md` (adapt the template).
4. Point your AI agent to the root `AUTOIMPROVE.md`—it handles the rest!

### Example Routing Table
| Task | Go to | Read | Notes |
|------|-------|------|-------|
| Research ideas | /research | AUTOIMPROVE.md | Gather data and validate hypotheses |
| Write code | /implement | AUTOIMPROVE.md | Build features with tests |

## Example Project

See the `seizure-detection/` worktree (not included in this repo for brevity, but available in the development setup): A complete seizure detection system built with AutoImprove.

- Root `AUTOIMPROVE.md`: Project navigation and metrics.
- Workspaces: `research/`, `implement/`, `test/`, etc., each with self-contained `AUTOIMPROVE.md`.
- Demonstrates recursive improvement on real EEG data.

For the full example, set up the worktree as described in the docs.

## Why AutoImprove?

- **Agent Superpower**: Turns AI agents into autonomous project managers.
- **Human-AI Synergy**: Provides structure for collaboration without micromanagement.
- **Scalable**: Works for solo projects or teams; nests infinitely.
- **Inspired by Best Practices**: Combines Jake's workflow architecture with Karpathy's self-research loops.

## Installation

No installation—clone the repo and copy the template. For code projects, manage dependencies separately.

## Usage

- **For Agents**: Read `AUTOIMPROVE.md`, use routing to navigate, evaluate rules, update files.
- **For Humans**: Edit markdown to guide agents; monitor logs for progress.
- **Customization**: Adapt template for your domain (e.g., add custom rules/metrics).

## Contributing

1. Read root `AUTOIMPROVE.md`.
2. Use routing to find workspace.
3. Update `AUTOIMPROVE.md` files.
4. PR with changes.

## License

MIT License - see LICENSE.

## Inspiration & Credits

- **Jake van der Plas**: Folder structure for AI workflows.
- **Andrej Karpathy**: Autoresearch mechanism with evaluation levers.
- **Open-Source Community**: For markdown-based tools and AI frameworks.

## Roadmap

- Community templates for different domains.
- Tool integrations for automated rule evaluation.
- Case studies from real projects.

---

**Ready to supercharge your projects?** Drop AutoImprove in and watch AI agents autonomously improve your work! 🚀