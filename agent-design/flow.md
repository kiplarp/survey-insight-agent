# Agent flow

1. User uploads survey comments CSV.
2. Assistant classifies each comment by theme, sentiment, urgency, and department.
3. Assistant drafts short summaries for business users.
4. If a comment includes safety, privacy, conduct, or ambiguity, route to human review.
5. Log outcome for KPI tracking.

## Fallback rules
- If confidence is low, mark for manual coding.
- If multiple themes conflict, escalate.
- If comment contains sensitive risk language, do not finalize automatically.
