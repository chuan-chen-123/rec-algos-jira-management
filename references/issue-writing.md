# Templates and examples

Use only the sections the work needs. Braced slots below are template inputs, not text to publish. Remove unused sections and resolve or explicitly qualify unknown facts.

## Story

**Summary:** `{Verb + concrete outcome or artifact}`

```markdown
{Problem or current behavior. What changes and why; include the relevant boundary.}

### Acceptance criteria
- {Observable result and conditions, with the evidence or comparison needed.}
- {Material regression, failure or eligibility check, when relevant.}
- {Artifact, handoff or decision that completes this deliverable.}

### Technical context
{Essential contract, constraint or implementation context. Omit when unnecessary.}

### Dependencies and evidence
{Required input or linked design, experiment, code or readout. Omit when unnecessary.}
```

Store assignee, Team, label, epic and fix version in their fields. A description may explain a concrete dependency or a role distinction without duplicating the entire metadata record.

Use beneficiary-centered user-story wording when helpful; technical work does not need a fictional end user.

## Epic

**Summary:** `{Coherent outcome or agreed group / area}`

```markdown
{Why this work exists, the beneficiary and intended result or decision.}

### Workstreams
- **{First distinct workstream}:** {Scope and boundary.}
- **{Second distinct workstream}:** {Scope and boundary.}

### Dependencies and decisions
{Concrete partner/input, current readiness and next decision, where material.}

### Completion
- {Evidence that accepted deliverables meet their respective criteria.}
- {Disposition of remaining work and any rollout or operating handoff.}
```

An epic covering several workstreams should explain each one proportionately. Expand acronyms within the relevant workstream. Keep one accountable delivery home for shared work.

When the request involves funding or prioritization, include the verified sponsoring initiative, full delivery/review/operating effort, capacity constraints, displaced work and next continue/pivot/stop decision. Reference the team's supplied planning policy once; do not invent funding, staffing, dates or allocation percentages. Routine ticket creation does not require manufacturing a business case.

## Tailor acceptance to the deliverable

| Work | Useful acceptance boundary |
|---|---|
| Experiment design | Hypothesis, eligible population, treatment/control, primary outcome, guardrails, sample/power and analysis plan are reviewed; unresolved launch dependencies are clear. |
| Experiment launch | Intended assignment/exposure and metric capture validated, relevant QA/monitoring/recovery ready, actual test-start evidence recorded. |
| Analysis/readout | Reproducible definitions and methods, results with uncertainty and limitations, and a Product decision handoff. Null or harmful results can complete the analysis. |
| Research | Named uncertainty, candidate/baseline on a defined evaluation set, limitations and a supported next decision. Production feasibility or positive lift is not guaranteed. |
| Migration/infrastructure | Defined consumer contract, parity/regression checks, staged deployment or cutover, measured evidence, recovery and operating handoff as applicable. |
| AI enablement | One bounded workflow, reference outcomes, correctness/unsupported-response checks, measured time or effort and a scale/revise/stop decision. |
| Defect-correction Story | Expected versus actual behavior, reproduction/evidence, bounded correction and relevant regressions. |

### Example: migration Story

**Summary:** Validate and cut over the training-data source

Use the accepted source in model training while preserving the agreed data and model-quality contracts.

**Acceptance criteria**

- Compare candidate and existing sources on representative schema, coverage and training distributions.
- Validate the staging ETL and model training; record backtest results and any reason to hold.
- For an accepted cutover, link deployment and recovery evidence and the operating handoff.

### Example: research Story

**Summary:** Evaluate the outfit-defect judge on reviewed examples

Determine whether the candidate judge captures the agreed visual defects reliably enough for the next integration decision.

**Acceptance criteria**

- Define a versioned evaluation set with provenance, reviewed labels and representative defect/non-defect cases.
- Compare candidate outputs with those labels, reporting false positives, false negatives and material coverage limitations.
- Publish reproducible results and an integrate, revise or stop recommendation; keep unknown thresholds unconfirmed.

### Example: epic with several workstreams

**Summary:** Outfit quality and coverage

Improve defect detection and ensure outfit generation respects the accepted composition and eligibility rules.

**Workstreams**

- **LLM-as-a-Judge:** evaluate visual defect detection and its required data/model validation.
- **Generation rules:** investigate template behavior and reconcile unintended differences after confirming Product intent.
- **Diagnostics and coverage:** expose classification/hydration failures and validate the agreed kept-item and assortment behavior.

**Completion**

- Accepted changes have representative quality/regression evidence and a reviewed decision.
- Remaining implementation or operating obligations are tracked in the appropriate child tickets.

These examples are illustrative; they are not preapproved backlog items or delivery commitments.
