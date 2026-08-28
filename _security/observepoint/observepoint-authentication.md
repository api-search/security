---
api_key_in:
- header
api_specs:
- filename: observepoint-v3-api-openapi.yml
  format: yaml
  label: ObservePoint V3 API
  slug: observepoint-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observepoint/refs/heads/main/openapi/observepoint-v3-api-openapi.yml
- filename: observepoint-grid-reports-api-openapi.yml
  format: yaml
  label: ObservePoint Grid Reporting API
  slug: observepoint-grid-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observepoint/refs/heads/main/openapi/observepoint-grid-reports-api-openapi.yml
- filename: observepoint-v2-api-openapi.yml
  format: yaml
  label: ObservePoint V2 API
  slug: observepoint-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observepoint/refs/heads/main/openapi/observepoint-v2-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Observepoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: ObservePoint secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ObservePoint
provider_slug: observepoint
scheme_count: 1
schemes:
- description: 'Use the `Authorization` header in your requests with ObservePoint API key as header value.


    Example: `Authorization: abc123...def456`'
  in: header
  name: API_Key
  parameter: Authorization
  sources:
  - openapi/observepoint-grid-reports-api-openapi.yml
  - openapi/observepoint-v2-api-openapi.yml
  - openapi/observepoint-v3-api-openapi.yml
  type: apiKey
slug: observepoint-authentication
source_filename: observepoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://api-docs.observepoint.com/ (Getting Started > Authentication); corroborated by securitySchemes in openapi/observepoint-v3-api-openapi.yml, openapi/observepoint-grid-reports-api-openapi.yml, openapi/observepoint-v2-api-openapi.yml\ndocs: https://api-docs.observepoint.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Single auth model across every ObservePoint API surface (v2, v3 and the Grid Reporting API): a\n    user-level API key sent in the Authorization header. There is no OAuth 2.0, no OpenID Connect and\n    no scope surface, so scopes/ is intentionally absent for this provider.\nschemes:\n- name: API_Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Use the `Authorization` header in your requests with ObservePoint API key as header value.\n\n    Example: `Authorization: abc123...def456`\n\
  \  sources:\n  - openapi/observepoint-grid-reports-api-openapi.yml\n  - openapi/observepoint-v2-api-openapi.yml\n  - openapi/observepoint-v3-api-openapi.yml\ndocs_detail:\n  header: Authorization\n  prefix: api_key\n  documented_form: 'Authorization: api_key YOUR_API_KEY_HERE'\n  note: >-\n    The published Getting Started guide documents the header value with an `api_key ` prefix\n    (\"Authorization: api_key YOUR_API_KEY_HERE\"), while the OpenAPI securityScheme description shows the\n    bare key (\"Authorization: abc123...def456\"). The docs example is the authoritative form; the spec\n    description is inconsistent with it. Recorded as published, not reconciled.\n  key_scope: user\n  key_issuance: Self-service from the user profile page in the ObservePoint app (app.observepoint.com/my-profile)\n  rotation: Documented for webhook signing secrets (POST /v3/webhooks/rotate-secret); no documented API-key rotation endpoint\n  source: https://api-docs.observepoint.com/\nobserved:\n- url:\
  \ https://api.observepoint.com/v2/api-docs\n  http_status: 401\n  body: Bearer token is absent\n  note: Unauthenticated request to an api.observepoint.com path returns 401 with a plain-text body.\n  probed: '2026-08-26'\nwebhook_authentication:\n  mechanism: HMAC-SHA256 request signature\n  header: ObservePoint-Signature\n  format: t=<unix-timestamp>,sigv1=<base64 HMAC-SHA256 of \"<timestamp>.<raw-body>\">\n  secret_provisioning: POST https://api.observepoint.com/v3/webhooks/rotate-secret (Admin permission required; secret shown once)\n  source: https://api-docs.observepoint.com/sections/webhook\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/observepoint/refs/heads/main/authentication/observepoint-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Web Governance
- Tag Management
- Analytics Validation
- Privacy Compliance
- Consent Management
- Web Accessibility
- Data Quality
- Marketing Technology
- Website Auditing
- Digital Analytics
- Webhooks
---
