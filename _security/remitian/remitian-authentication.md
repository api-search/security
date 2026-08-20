---
api_key_in: []
api_specs:
- filename: remitian-accounts-api-openapi.yml
  format: yaml
  label: Remitian Accounts API
  slug: remitian-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/openapi/remitian-accounts-api-openapi.yml
- filename: remitian-audit-logs-api-openapi.yml
  format: yaml
  label: Remitian Audit Logs API
  slug: remitian-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/openapi/remitian-audit-logs-api-openapi.yml
- filename: remitian-jurisdictions-api-openapi.yml
  format: yaml
  label: Remitian Jurisdictions API
  slug: remitian-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/openapi/remitian-jurisdictions-api-openapi.yml
- filename: remitian-payments-api-openapi.yml
  format: yaml
  label: Remitian Payments API
  slug: remitian-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/openapi/remitian-payments-api-openapi.yml
- filename: remitian-webhooks-api-openapi.yml
  format: yaml
  label: Remitian Webhooks API
  slug: remitian-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/openapi/remitian-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Remitian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Remitian secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Remitian
provider_slug: remitian
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: API key authentication using a Bearer token provided by Remitian during partner onboarding.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/remitian-tax-payment-openapi.yml
  type: http
slug: remitian-authentication
source_filename: remitian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/remitian-tax-payment-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: API key authentication using a Bearer token provided by Remitian during partner\n    onboarding.\n  sources:\n  - openapi/remitian-tax-payment-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remitian/refs/heads/main/authentication/remitian-authentication.yml
summary_line: http · 1 scheme
tags:
- Tax
- Payments
- Fintech
- Accounting
- Webhook
- Embedded Payments
---
