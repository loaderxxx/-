# CURSOR BOOTSTRAP

1. Read `AGENTS.md`, this file, `collaboration/AI_TEAM_PROTOCOL.md` and `collaboration/AGENT_STATE.md`.
2. Read the repository README / manifest and only the task-relevant files.
3. Refresh `main`, `agent/cursor`, `agent/chatgpt` and inspect related Issues/PRs.
4. Treat `main` as canonical and `agent/cursor` as the Cursor working lane.
5. Implement only the assigned scope; use `work/cursor/<task-id>-<slug>` for substantial isolated work.
6. Test and verify actual results.
7. Commit and push the working branch; communicate through Issue/PR using the PR template.
8. Never silently overwrite another agent's material work or push main without explicit owner authorization.
9. Never commit credentials, tokens, passwords or prohibited private data.
10. After integration, refresh from `main` before dependent work.

## Cost-aware multitask orchestration

When this repository is operated from Claude Code/Fable, Fable is the orchestration and judgment layer.

For substantial work:
- decompose the task into auditable subtasks before executing;
- parallelize independent subtasks;
- create specialized worker agents for bounded actions;
- route routine/mechanical work to the cheapest capable worker;
- prefer the latest available Grok worker for cost-efficient general implementation/execution; xAI currently documents `grok-4.6` as its frontier coding/agentic model;
- keep architecture, security, conflict resolution and final acceptance at the strongest reasoning layer;
- independently verify worker output before integration;
- escalate failed, ambiguous or high-risk work to a stronger worker/Fable.

Read `collaboration/AI_ORCHESTRATION_ROUTING.md` for the detailed policy.
