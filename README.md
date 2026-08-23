# Survey Insight Agent

A mock enterprise AI assistant that helps internal teams analyze open-ended survey feedback, classify key themes, draft manager-ready summaries, and escalate sensitive or ambiguous cases for human review.

## Business problem

Teams often receive large volumes of open-ended survey comments that are time-consuming to code and summarize manually. This project shows how an AI-assisted workflow can speed up first-pass analysis while preserving governance, fallback behavior, and human oversight.

## Project goals

- Turn raw survey comments into structured business insights.
- Classify comments by theme, sentiment, urgency, and department.
- Draft short manager-ready summaries from coded feedback.
- Escalate sensitive or unclear cases for human review.
- Track workflow metrics such as auto-classification rate and escalation rate.

## Example workflow

1. Upload or import survey comments from a CSV file.
2. Classify each comment by theme, sentiment, urgency, and department.
3. Draft a short summary for the relevant business team.
4. Route ambiguous or sensitive comments to human review.
5. Log outputs for KPI and adoption tracking.

## Repository structure

```text
survey-insight-agent/
├── README.md
├── data/
│   └── sample_survey_comments.csv
├── prompts/
│   ├── classify.md
│   ├── summarize.md
│   └── escalate.md
├── agent-design/
│   └── flow.md
├── governance/
│   └── ai-safety-notes.md
├── examples/
│   ├── sample-inputs.md
│   └── sample-outputs.md
└── dashboard/
    └── kpi-notes.md
```

## Governance controls

- Approved source: survey export or mock survey dataset only.
- No personal data enrichment.
- Human review required for safety, legal, reputational, privacy, or conduct-related issues.
- All AI-generated summaries are treated as draft outputs.
- Low-confidence or multi-theme comments are marked for manual review.

## Skills demonstrated

- Prompt design
- Survey coding workflow design
- Feedback classification
- AI governance and fallback planning
- Escalation logic
- Business reporting
- KPI thinking for internal AI tools

## Sample use case

A guest experience or marketing team receives dozens of open-ended comments from a post-visit survey. Instead of manually coding every response from scratch, the assistant performs a first-pass classification, drafts a concise summary for department managers, and flags high-risk or unclear comments for review.

## Planned files

### `data/sample_survey_comments.csv`
Mock survey comments with fields such as:
- `comment_id`
- `comment`
- `theme`
- `sentiment`
- `urgency`
- `department`
- `needs_human_review`
- `review_reason`
- `manager_summary`
- `suggested_action`

### `prompts/classify.md`
Prompt template for theme, sentiment, urgency, and department classification.

### `prompts/summarize.md`
Prompt template for producing short manager-ready summaries.

### `prompts/escalate.md`
Prompt template for deciding whether a comment should be routed to human review.

## Next steps

- Add a 25-100 row sample survey dataset.
- Upload prompt templates for classification, summarization, and escalation.
- Add example raw comments and AI-generated outputs.
- Create a simple KPI dashboard in Power BI or Excel.
- Optionally add a Python script for automated classification.

## Why this project

This project is designed as a practical AI workflow case study rather than a generic chatbot demo. The focus is on usable business processes, controlled outputs, escalation behavior, and internal reporting.
