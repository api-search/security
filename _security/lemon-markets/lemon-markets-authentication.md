---
api_key_in: []
api_specs:
- filename: lemon-markets-brokerage-openapi.json
  format: json
  label: lemon.markets Brokerage API
  slug: brokerage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemon-markets/refs/heads/main/openapi/lemon-markets-brokerage-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lemon Markets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lemon Markets secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lemon Markets
provider_slug: lemon-markets
scheme_count: 1
schemes:
- applied: global (root-level security requirement)
  format: Bearer <api-key>
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lemon-markets-brokerage-openapi.json
  type: http
slug: lemon-markets-authentication
source_filename: lemon-markets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lemon-markets-brokerage-openapi.json\ndocs:\n- https://developer.lemon.markets/docs/getting-started\n- https://developer.lemon.markets/docs/webhooks-setup\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  scopes: none\n  model: >-\n    A single partner-scoped bearer API key. There is no OAuth, no OpenID Connect, no scope surface and\n    no mutual TLS. Authorisation is partner-wide, and the acting principal is carried per request in\n    mandatory data-privacy headers rather than in the token.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  applied: global (root-level security requirement)\n  header: Authorization\n  format: Bearer <api-key>\n  sources:\n  - openapi/lemon-markets-brokerage-openapi.json\nrequired_request_headers:\n- name: LMG-Data-Privacy-Access-Principal\n  in: header\n  required: true\n  applies_to: customer-data operations\n  description: >-\n    Identifies the\
  \ principal (human or system) on whose behalf the request is made. Declared as a\n    required OpenAPI parameter, so requests omitting it fail.\n- name: LMG-Data-Privacy-Access-Justification\n  in: header\n  required: true\n  applies_to: customer-data operations\n  description: >-\n    Free-text justification for accessing customer data in this request, recorded alongside the\n    principal for data-protection auditing.\nkey_management:\n  issuance: issued during partner onboarding; the API is invite-only with no self-service signup\n  rotation: not documented publicly\n  test_vs_live_prefix: not documented; environments are separated by hostname\n  scopes_or_permissions: none published\nwebhook_authentication:\n  direction: inbound to the partner\n  mechanism: HMAC-SHA256 signature in the LMG-Signature header\n  secret: per-webhook signature_secret returned at registration\n  detail: asyncapi/lemon-markets-brokerage-webhooks.yml\nnot_supported:\n- oauth2\n- openIdConnect\n- apiKey query\
  \ or cookie parameters\n- mutualTLS\n- sender-constrained / proof-of-possession tokens\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemon-markets/refs/heads/main/authentication/lemon-markets-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Brokerage
- Trading
- Investing
- Securities
- Financial Services
- Banking as a Service
- Fintech
- Wealth Management
- Embedded Finance
- Germany
---
