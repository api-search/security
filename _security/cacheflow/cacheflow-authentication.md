---
api_key_in: []
api_specs:
- filename: cacheflow-api-openapi.yml
  format: yaml
  label: Cacheflow API
  slug: cacheflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cacheflow/refs/heads/main/openapi/cacheflow-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cacheflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cacheflow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cacheflow
provider_slug: cacheflow
scheme_count: 1
schemes:
- description: Static, long-lived API token minted per organization from the Cacheflow web app (Settings -> API -> create an API token). Presented as an RFC 6750 bearer token.
  format: 'Authorization: Bearer <api-token>'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://github.com/getcacheflow/api-examples/blob/HEAD/SETUP.md
  - https://github.com/getcacheflow/api-examples/blob/HEAD/src/api/index.ts
  type: http
slug: cacheflow-authentication
source_filename: cacheflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://github.com/getcacheflow/api-examples/blob/HEAD/SETUP.md\ndocs: https://developer.getcacheflow.com/docs/create-an-api-token\nnote: >-\n  The harvested OpenAPI (openapi/_original/cacheflow-openapi.json) declares NO\n  components.securitySchemes and no operation-level security[], so nothing could be\n  derived from the contract. The auth model below is taken verbatim from Cacheflow's\n  own public GitHub org (github.com/getcacheflow/api-examples), which documents the\n  token, the header, and the tenant-routing Host header, and is corroborated by the\n  token-management operations that exist in the spec itself.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  declared_in_spec: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <api-token>'\n  description: >-\n    Static, long-lived\
  \ API token minted per organization from the Cacheflow web app\n    (Settings -> API -> create an API token). Presented as an RFC 6750 bearer token.\n  sources:\n  - https://github.com/getcacheflow/api-examples/blob/HEAD/SETUP.md\n  - https://github.com/getcacheflow/api-examples/blob/HEAD/src/api/index.ts\ntenant_routing:\n  required: true\n  mechanism: Host header\n  form: '<org-flow-domain>.api.getcacheflow.com'\n  sandbox_form: '<org-flow-domain>.api.sandbox.getcacheflow.com'\n  description: >-\n    Cacheflow routes API calls to a per-organization domain. Callers send the base URL\n    plus an explicit Host header naming their org's flow domain; the token alone is not\n    sufficient. Recorded verbatim from api-examples/SETUP.md and src/api/index.ts.\ntoken_management:\n  described_in_spec: true\n  operations:\n  - operationId: getAllTokens\n    method: GET\n    path: /api/latest/settings/api/tokens\n    summary: List API tokens\n  - operationId: addToken\n    method: POST\n    path:\
  \ /api/latest/settings/api/tokens\n    summary: Create an API token\n  - operationId: removeToken\n    method: DELETE\n    path: /api/latest/settings/api/tokens/{id}\n    summary: Delete an token\n  ui_path: Settings -> API\nsso:\n  described_in_spec: true\n  note: >-\n    The spec exposes GET /api/latest/auth/providers (getProviderList, \"List SSO Providers\")\n    and SAML-related error codes, indicating tenant SSO for the web application. This is\n    end-user sign-in, not API authentication.\noauth2_note: >-\n  The spec's oauth endpoints under /api/latest/settings/integrations/oauth/* are OUTBOUND\n  connectors (Cacheflow authorizing itself against QuickBooks, Salesforce, HubSpot, Slack,\n  DocuSign, Stripe, Plaid). Cacheflow does NOT publish an OAuth 2.0 authorization server\n  for third-party API clients, so scopes/ is intentionally absent.\nerror_codes_related:\n  - BEARER_TOKEN_INVALID_equivalent: BearerTokenInvalid\n  - NOT_AUTHORIZED_TO_ACCESS_ENTITY\n  - AUTH_CODE_INVALID\n\
  \  - AUTH_CODE_MAX_ATTEMPTS\nx-evidence:\n- url: https://raw.githubusercontent.com/getcacheflow/api-examples/HEAD/SETUP.md\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://raw.githubusercontent.com/getcacheflow/api-examples/HEAD/src/api/index.ts\n  http_status: 200\n  fetched: '2026-08-13'\nx-status-note: >-\n  Cacheflow was acquired by HubSpot in 2024. As of 2026-08-13 api.getcacheflow.com and\n  api.sandbox.getcacheflow.com no longer resolve (NXDOMAIN), so no token can be exercised\n  against a live host. The auth contract is recorded as the provider published it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cacheflow/refs/heads/main/authentication/cacheflow-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Billing
- Subscription
- CPQ
- Quote-to-Cash
- Payments
- Software-as-a-Service
- Invoicing
- Revenue Operations
- E-Signature
- Retired API
---
