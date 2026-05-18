# Lead.AI Lead Scoring API

A JSON API that scores leads, explains priority factors, and helps teams focus follow-up on the best opportunities.

## Product Status

Prototype / MVP

This repository is public and suitable for product planning, documentation review, and future implementation. It should not be described as production-ready until working code, tests, deployment steps, and security controls are in place.

## Problem Solved

Businesses do not know which leads deserve priority follow-up.

## Target Users

- Sales teams
- CRM builders
- Lead generation agencies
- Small business operators
- Growth teams

## Key Features

- Lead scoring endpoint
- Lead qualification rules
- AI-generated lead summary
- Risk/opportunity score
- JSON API
- Input validation
- API documentation
- Test examples

## Tech Stack

- Python
- FastAPI
- Pydantic
- scikit-learn-ready structure

## Architecture Overview

The intended architecture separates product UI, backend workflows, AI orchestration, data storage, integrations, and operational controls.

Core layers:

- User experience layer for business users and administrators.
- API or service layer for validation, workflow execution, and integrations.
- AI layer for prompts, scoring, summaries, recommendations, or decision support.
- Data layer for leads, conversations, reports, scores, configuration, or audit records.
- Security layer for authentication, authorization, privacy, logging, and secret management.

See [Architecture](docs/ARCHITECTURE.md) for the detailed design direction.

## Setup Instructions

There is no complete runnable application in this repository yet unless implementation files have been added after this documentation pass.

Recommended future setup pattern:

```bash
cp .env.example .env
# install project dependencies after the stack is implemented
# run the local development server after package scripts are added
```

When code is added, update this section with exact install, development, test, lint, and build commands.

## Environment Variables

Configuration is documented in [.env.example](.env.example). Use placeholder names only in public files. Never commit real `.env` files, API keys, access tokens, private credentials, customer exports, or private datasets.

## Usage Flow

1. A lead record is submitted to the scoring endpoint.
2. The API validates the payload and applies qualification logic.
3. The response returns score, priority band, explanation factors, and suggested next action.
4. The calling system stores the result or routes the lead.

See [User Flow](docs/USER_FLOW.md) for more detail.

## Screenshots And Demo

Screenshots, demo links, and videos will be added after a working demo exists.

Suggested public assets:

- Product dashboard screenshot.
- Primary workflow screenshot.
- Short demo video or GIF.
- Deployment or live demo link, if available.

## Roadmap

See [Roadmap](docs/ROADMAP.md) and [MVP Plan](docs/MVP_PLAN.md).

Immediate next step: Create Pydantic schemas, deterministic scoring rules, and example API responses.

## Security Notes

- Do not commit secrets or private customer data.
- Validate user input before storage, scoring, AI processing, or external API calls.
- Avoid logging personally identifiable information.
- Add authentication and authorization before handling protected business data.

See [Security](docs/SECURITY.md).

## Responsible AI Notes

- Keep AI limitations visible to users and reviewers.
- Avoid unsupported claims about accuracy or reliability.
- Provide human review or handoff for sensitive, uncertain, or high-impact outcomes.
- Prefer explainable outputs for scores, recommendations, and risk signals.

## Related Lead.AI Products

- [Lead.AI Platform](https://github.com/Lead-AI-US/lead-ai-platform)
- [Lead.AI Business Audit](https://github.com/Lead-AI-US/lead-ai-business-audit)
- [Lead.AI WhatsApp Agent](https://github.com/Lead-AI-US/lead-ai-whatsapp-agent)
- [Lead.AI Website Chatbot](https://github.com/Lead-AI-US/lead-ai-website-chatbot)
- [Lead.AI Lead Scoring API](https://github.com/Lead-AI-US/lead-ai-lead-scoring-api)
- [Lead.AI Prompt Vault](https://github.com/Lead-AI-US/lead-ai-prompt-vault)
- [Lead.AI Firebase SaaS Starter](https://github.com/Lead-AI-US/lead-ai-firebase-saas-starter)
- [Lead.AI Fraud Shield](https://github.com/Lead-AI-US/lead-ai-fraud-shield)

## Author

Founded by Arun Kumar Gharami.  
Website: https://www.lead-ai.us  
GitHub: https://github.com/Arungharami

## License

See [LICENSE](LICENSE). A final license should be selected before accepting external contributions or publishing reusable code.
