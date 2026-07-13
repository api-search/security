---
api_key_in:
- query
api_specs:
- filename: email-verifier-api-openapi.yml
  format: yaml
  label: Email Verifier API Verification
  slug: verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/email-verifier-api/refs/heads/main/openapi/email-verifier-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Email Verifier Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Email Verifier API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Email Verifier API
provider_slug: email-verifier-api
scheme_count: 1
schemes:
- description: 'API key issued at signup. Pass as the `apiKey` query string parameter on every

    request. Treat the key as a credential and rotate from the customer dashboard

    if exposed.'
  in: query
  name: apiKeyQuery
  parameter: apiKey
  sources:
  - openapi/email-verifier-api-openapi.yml
  type: apiKey
slug: email-verifier-api-authentication
source_filename: email-verifier-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/email-verifier-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: |-\n    API key issued at signup. Pass as the `apiKey` query string parameter on every\n    request. Treat the key as a credential and rotate from the customer dashboard\n    if exposed.\n  sources:\n  - openapi/email-verifier-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/email-verifier-api/refs/heads/main/authentication/email-verifier-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Verification
- Deliverability
- SMTP Check
- Bounce Prevention
- Lead Validation
- Disposable Detection
- Spam Trap Detection
- Catch-All Detection
- Greylisting
- Role Account Detection
- Typo Suggestion
- B2B Lead Scoring
---
