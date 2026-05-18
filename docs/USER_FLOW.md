# User Flow

## Primary User

Sales teams

## Primary Flow

1. A lead record is submitted to the scoring endpoint.
2. The API validates the payload and applies qualification logic.
3. The response returns score, priority band, explanation factors, and suggested next action.
4. The calling system stores the result or routes the lead.

## Happy Path Outcome

The user receives a clear business result from Lead.AI Lead Scoring API without needing to understand the underlying AI or infrastructure.

## Failure And Handoff Paths

- If required data is missing, ask for the minimum additional information.
- If the AI output is uncertain, show a limitation or request human review.
- If an integration fails, preserve the input and show a recoverable error.
- If private data is involved, avoid exposing it in logs or public examples.

## Demo Requirements

- Use safe sample data.
- Show the main workflow end to end.
- Include one screenshot or short video after implementation.
