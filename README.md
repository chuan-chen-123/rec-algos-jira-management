# Rec Algos Jira Management

A standalone skill for drafting, creating and reviewing Rec Algos Jira epics, stories and subtasks. It runs independently of Virtual Me and uses each teammate's own Jira connection.

## What it includes

- Epic → Story → Subtask structure and concise writing templates.
- Checks for assignee, work-type label, parent epic, Team, fix version and Product-priority links.
- Recommendation Algorithms team conventions.
- Fiscal-quarter scheduling: FY27Q2 is November 2026–January 2027; FY27Q3 is February–April 2027. The intended work quarter determines the version.
- Guidance for preserving original tickets, comments, attachments and subtask history.

## Install in Codex

After receiving access to this private repository, choose one method.

**Clone into your skills directory:**

```sh
git clone https://github.com/chuan-chen-123/rec-algos-jira-management.git ~/.codex/skills/rec-algos-jira-management
```

If you use a custom `CODEX_HOME`, clone into its `skills/rec-algos-jira-management` directory instead.

**Or download:** select **Code → Download ZIP**, extract it, rename the extracted folder to `rec-algos-jira-management`, and place it in your Codex skills directory. Keep `SKILL.md`, `agents/` and `references/` together.

Reload the skill list or start a new chat if needed. See [installation details](INSTALL.md) for other SKILL.md-compatible agents.

## Use it

Connect your own Atlassian account for live Jira actions. Drafting does not require a Jira connection.

> Use $rec-algos-jira-management to draft a story for this experiment readout. Show me the draft before creating it.

> Use $rec-algos-jira-management to create this approved infrastructure story for FY27Q3 under the existing infrastructure epic. Leave the assignee unassigned.

> Use $rec-algos-jira-management to review these Jira tickets and fix supported field or description problems.

## Files

- [Skill instructions](SKILL.md)
- [Team conventions](references/team-conventions.md)
- [Story and epic templates](references/issue-writing.md)
- [Fiscal-quarter mapping](references/fiscal-quarters.md)
- [Live Jira workflow](references/jira-workflow.md)
- [History and hierarchy](references/history-and-hierarchy.md)

This repository contains no credentials or private Virtual Me files. Installing the skill does not grant Jira access. Team conventions are working guidance; current explicit instructions and verified project settings take precedence.
