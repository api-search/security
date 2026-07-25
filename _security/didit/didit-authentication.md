---
api_key_in:
- header
api_specs:
- filename: didit-billing-api-openapi.yml
  format: yaml
  label: Didit Billing API
  slug: didit-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-billing-api-openapi.yml
- filename: didit-businesses-api-openapi.yml
  format: yaml
  label: Didit Businesses API
  slug: didit-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-businesses-api-openapi.yml
- filename: didit-case-blueprints-api-openapi.yml
  format: yaml
  label: Didit Case Blueprints API
  slug: didit-case-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-case-blueprints-api-openapi.yml
- filename: didit-cases-api-openapi.yml
  format: yaml
  label: Didit Cases API
  slug: didit-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-cases-api-openapi.yml
- filename: didit-customization-api-openapi.yml
  format: yaml
  label: Didit Customization API
  slug: didit-customization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-customization-api-openapi.yml
- filename: didit-questionnaires-api-openapi.yml
  format: yaml
  label: Didit Questionnaires API
  slug: didit-questionnaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-questionnaires-api-openapi.yml
- filename: didit-regulatory-reports-api-openapi.yml
  format: yaml
  label: Didit Regulatory Reports API
  slug: didit-regulatory-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-regulatory-reports-api-openapi.yml
- filename: didit-report-templates-api-openapi.yml
  format: yaml
  label: Didit Report Templates API
  slug: didit-report-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-report-templates-api-openapi.yml
- filename: didit-session-api-openapi.yml
  format: yaml
  label: Didit Session API
  slug: didit-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-session-api-openapi.yml
- filename: didit-sessions-api-openapi.yml
  format: yaml
  label: Didit Sessions API
  slug: didit-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-sessions-api-openapi.yml
- filename: didit-standalone-apis-api-openapi.yml
  format: yaml
  label: Didit Standalone APIs API
  slug: didit-standalone-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-standalone-apis-api-openapi.yml
- filename: didit-system-api-openapi.yml
  format: yaml
  label: Didit System API
  slug: didit-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-system-api-openapi.yml
- filename: didit-transactions-api-openapi.yml
  format: yaml
  label: Didit Transactions API
  slug: didit-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-transactions-api-openapi.yml
- filename: didit-travel-rule-api-openapi.yml
  format: yaml
  label: Didit Travel Rule API
  slug: didit-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-travel-rule-api-openapi.yml
- filename: didit-users-api-openapi.yml
  format: yaml
  label: Didit Users API
  slug: didit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-users-api-openapi.yml
- filename: didit-webhook-api-openapi.yml
  format: yaml
  label: Didit Webhook API
  slug: didit-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-webhook-api-openapi.yml
- filename: didit-workflows-api-openapi.yml
  format: yaml
  label: Didit Workflows API
  slug: didit-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Didit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Didit secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Didit
provider_slug: didit
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/didit-openapi-original.json
  type: apiKey
- description: Short-lived scoped token minted by your backend via POST /v3/transactions/sdk-token/. Used by the Didit SDKs on the device-facing /v1/transactions/ endpoints.
  in: header
  name: TransactionTokenAuth
  parameter: X-Transaction-Token
  sources:
  - openapi/didit-openapi-original.json
  type: apiKey
- description: Short-lived token returned in the `session_token` field of POST /v3/session/. Used by the hosted verification flow (and custom sandbox UIs) to call session-scoped endpoints on behalf of the verifying user, without your server-side API key.
  in: header
  name: SessionTokenAuth
  parameter: Session-Token
  sources:
  - openapi/didit-openapi-original.json
  type: apiKey
slug: didit-authentication
source_filename: didit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/didit-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/didit-openapi-original.json\n- name: TransactionTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Transaction-Token\n  description: Short-lived scoped token minted by your backend via POST /v3/transactions/sdk-token/.\n    Used by the Didit SDKs on the device-facing /v1/transactions/ endpoints.\n  sources:\n  - openapi/didit-openapi-original.json\n- name: SessionTokenAuth\n  type: apiKey\n  in: header\n  parameter: Session-Token\n  description: Short-lived token returned in the `session_token` field of POST /v3/session/.\n    Used by the hosted verification flow (and custom sandbox UIs) to call session-scoped endpoints\n    on behalf of the verifying user, without your server-side API key.\n  sources:\n  - openapi/didit-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/authentication/didit-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Identity
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Compliance
- Biometrics
- Transaction Monitoring
- Crypto
---
