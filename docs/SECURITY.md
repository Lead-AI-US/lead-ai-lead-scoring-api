# Security

## Status

Planned

Security controls must be reviewed again when API code and scoring logic are added.

## Requirements

- Do not commit API secrets, `.env` files, private datasets, or customer exports.
- Require authentication for non-public scoring endpoints.
- Validate all lead inputs with structured schemas.
- Avoid logging personally identifiable information.
- Return explainable score factors without exposing sensitive model internals.
- Review model outputs for fairness, reliability, and misuse risk.

## Reporting

Report security concerns privately to the maintainer before public disclosure.
