---
api_key_in:
- header
api_specs:
- filename: emailrep-api-openapi.yml
  format: yaml
  label: EmailRep API
  slug: emailrep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailrep/refs/heads/main/openapi/emailrep-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Emailrep Authentication
name_suffix: Authentication
oauth_flows: []
overview: EmailRep secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EmailRep
provider_slug: emailrep
scheme_count: 1
schemes:
- description: EmailRep API key issued at https://emailrep.io/key. Free tier is available; the Commercial and Enterprise tiers raise the per-month and per-day quotas. The key is passed in the `Key` HTTP header on every request.
  in: header
  name: ApiKeyAuth
  parameter: Key
  sources:
  - openapi/emailrep-api-openapi.yml
  type: apiKey
slug: emailrep-authentication
source_filename: emailrep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/emailrep-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Key\n  description: EmailRep API key issued at https://emailrep.io/key. Free tier is available; the\n    Commercial and Enterprise tiers raise the per-month and per-day quotas. The key is passed\n    in the `Key` HTTP header on every request.\n  sources:\n  - openapi/emailrep-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailrep/refs/heads/main/authentication/emailrep-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Email
- Email Reputation
- Threat Intelligence
- Phishing
- Fraud Prevention
- Anti-Abuse
- Deliverability
- Risk Scoring
- Public APIs
---
