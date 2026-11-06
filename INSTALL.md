# Share and use this skill

This package contains the standalone Rec Algos Jira Management skill. It does not need Virtual Me, Chuan's memory files, calendar, transcripts, credentials or another local skill.

## Codex installation

Extract the ZIP, then copy the complete `rec-algos-jira-management` folder into your Codex skills directory:

- macOS/Linux default: `~/.codex/skills/rec-algos-jira-management/`
- If you configured `CODEX_HOME`, use its `skills/` directory instead.

Keep `SKILL.md`, `agents/` and `references/` together. Reload the skill list or start a new chat if your client has not picked up the new skill. For another agent that supports SKILL.md packages, use that agent's documented skill-installation mechanism.

For live Jira actions, connect your own Atlassian account with the access needed for your task. Installing this skill does not connect Jira or grant permissions. You can draft stories and epics without a connection.

## Example requests

- `Use $rec-algos-jira-management to draft a story for this experiment readout. Show me the draft before creating it.`
- `Use $rec-algos-jira-management to create this approved migration Story under the existing infrastructure epic. Assign it to the named owner and use the release I supplied.`
- `Use $rec-algos-jira-management to draft an epic covering these related workstreams and suggest independently accepted child deliverables.`
- `Use $rec-algos-jira-management to audit these issue keys, fix supported field/description problems, and leave unassigned tickets unassigned.`

New work uses Epic → Story → Subtask. Team defaults live in `references/team-conventions.md`; templates live in `references/issue-writing.md`; fiscal-quarter mapping lives in `references/fiscal-quarters.md`. Adapt those defaults when intentionally using the skill for another team. Supply current project, owner, release and Product context rather than relying on a dated roadmap.
