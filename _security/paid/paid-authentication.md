---
api_key_in: []
api_specs:
- filename: paid-v2.json
  format: json
  label: Paid API v2
  slug: paid-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-v2.json
- filename: paid-v1.json
  format: json
  label: Paid API v1
  slug: paid-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-v1.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Paid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paid
provider_slug: paid
scheme_count: 1
schemes:
- description: API key authentication using a Bearer token. Keys are prefixed `paid_` and issued from the Paid app.
  header: 'Authorization: Bearer paid_xxx'
  issued_at: https://app.paid.ai/settings/api-keys
  key_prefix: paid_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paid-v1.json
  - openapi/paid-v2.json
  type: http
slug: paid-authentication
source_filename: paid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/paid-v1.json, openapi/paid-v2.json, https://docs.paid.ai/documentation/getting-started/quickstart\ndocs: https://docs.paid.ai/cli/cli/command-reference\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key authentication using a Bearer token. Keys are prefixed `paid_`\n    and issued from the Paid app.\n  key_prefix: paid_\n  header: 'Authorization: Bearer paid_xxx'\n  issued_at: https://app.paid.ai/settings/api-keys\n  sources:\n  - openapi/paid-v1.json\n  - openapi/paid-v2.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/authentication/paid-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Billing
- Monetization
- Payments
- Usage-Based Pricing
- AI Agents
- FinOps
---
