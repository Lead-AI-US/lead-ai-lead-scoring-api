# API Spec

## Status

Prototype / MVP

This API spec is a planning document. Endpoints should be treated as proposed until code and tests are added.

## API Principles

- Validate every request with structured schemas.
- Return JSON responses with clear error messages.
- Require authentication before handling protected business data.
- Avoid logging personally identifiable information.
- Include explanation factors for AI-generated scores, recommendations, or risk outputs.

## Proposed Endpoint

`POST /v1/leads/score`

### Example Request

```json
{"lead":{"name":"Sample Lead","source":"website","budget":"medium","urgency":"high"}}
```

### Example Response

```json
{"score":82,"priority":"high","factors":["high urgency","clear source"],"next_action":"Call within 1 business hour"}
```

## Error Format

```json
{"error":"validation_error","message":"Describe the missing or invalid field","request_id":"demo-request-id"}
```

## Security Requirements

- Add authentication before customer use.
- Keep API keys and provider credentials server-side.
- Rate limit public or webhook-facing endpoints.
- Document data retention and logging behavior before production use.
