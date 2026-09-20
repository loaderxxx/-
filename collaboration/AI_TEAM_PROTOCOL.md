# AI TEAM PROTOCOL

Shared coordination bus for the human owner, Cursor and ChatGPT/JARVIS.

Roles:
- Cursor — Lead Engineering Agent.
- ChatGPT/JARVIS — Systems Architect / Chief of Staff.
- Human owner — final authority for strategic, legal/financial, public, destructive and irreversible matters.

Branches:
- main = canonical integrated state.
- agent/cursor = Cursor lane.
- agent/chatgpt = ChatGPT lane.
- work/<agent>/<task-id>-<slug> = isolated task branch.

Loop:
FETCH → READ → PLAN → CHANGE → TEST → COMMIT → PUSH → PR/ISSUE → REVIEW → MERGE → FETCH

Issues are the default handoff channel; PRs are the integration/review channel.
Never silently overwrite material changes. Never commit secrets or prohibited private data.
Repository-specific rules and disclosure policies always apply.

Desired main protection: PR before merge, relevant checks/review, no force-push, no deletion. Enforcement must be verified in GitHub settings.
