---
api_key_in:
- header
api_specs:
- filename: rainforest-payments-openapi.yaml
  format: yaml
  label: Rainforest Payments API
  slug: rainforest-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest/refs/heads/main/openapi/rainforest-payments-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rainforest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rainforest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rainforest
provider_slug: rainforest
scheme_count: 1
schemes:
- bearerFormat: APIKey
  description: 'Provide the API key in the Authorization header with the `Bearer` prefix: `Authorization: Bearer {api_key}`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/rainforest-authentication-openapi.yaml
  - openapi/rainforest-deposits-openapi.yaml
  - openapi/rainforest-file_uploads-openapi.yaml
  - openapi/rainforest-forward_requests-openapi.yaml
  - openapi/rainforest-health-openapi.yaml
  - openapi/rainforest-merchants-openapi.yaml
  - openapi/rainforest-payments-openapi.yaml
  type: http
slug: rainforest-authentication
source_filename: rainforest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/rainforest-authentication-openapi.yaml, openapi/rainforest-payments-openapi.yaml\ndocs: https://docs.rainforestpay.com/docs/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  notes: >-\n    Rainforest uses API keys presented as HTTP Bearer tokens. Server-to-server calls\n    authenticate with a secret API key; embedded web/merchant Components authenticate\n    with a short-lived session token minted by POST /v1/sessions and scoped to a\n    specific config (payin, payment method, merchant onboarding, or reporting).\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: APIKey\n  description: >-\n    Provide the API key in the Authorization header with the `Bearer` prefix:\n    `Authorization: Bearer {api_key}`.\n  sources:\n  - openapi/rainforest-authentication-openapi.yaml\n  - openapi/rainforest-deposits-openapi.yaml\n  - openapi/rainforest-file_uploads-openapi.yaml\n\
  \  - openapi/rainforest-forward_requests-openapi.yaml\n  - openapi/rainforest-health-openapi.yaml\n  - openapi/rainforest-merchants-openapi.yaml\n  - openapi/rainforest-payments-openapi.yaml\nkey_types:\n- kind: api_key\n  usage: server-to-server\n  prefix_production: apikey_\n  prefix_sandbox: sbx_apikey_\n  managed_via: POST /v1/api_keys (create_api_key); can be disabled/enabled/deleted\n  docs: https://docs.rainforestpay.com/docs/authentication\n- kind: session_token\n  usage: embedded Components (frontend)\n  managed_via: POST /v1/sessions (create_session), DELETE /v1/sessions (delete_session)\n  scope: bound to a single config id (payin_config, payment_method_config, merchant_application, or report)\n  notes: Short-lived, safe to expose to the browser; never expose an API key to the frontend.\nversion_header:\n  name: Rainforest-Api-Version\n  scheme: date-based (e.g. 2024-10-16); requests default to the platform minimum API version\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainforest/refs/heads/main/authentication/rainforest-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Embedded Payments
- Payment Facilitator
- Payment Processing
- Vertical SaaS
- Fintech
- ACH
---
