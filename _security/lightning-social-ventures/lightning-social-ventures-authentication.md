---
api_key_in: []
api_specs:
- filename: lightning-social-ventures-lightning-reach-openapi.json
  format: json
  label: Lightning Reach API
  slug: lightning-reach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightning-social-ventures/refs/heads/main/openapi/lightning-social-ventures-lightning-reach-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Lightning Social Ventures Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightning Social Ventures declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Lightning Social Ventures
provider_slug: lightning-social-ventures
scheme_count: 0
schemes: []
slug: lightning-social-ventures-authentication
source_filename: lightning-social-ventures-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: https://api.lightningreach.org/docs\nnotes: >-\n  The published Lightning Reach API OpenAPI declares NO components.securitySchemes\n  and no operation-level security[], yet the API is fully authenticated: every\n  path on api.lightningreach.org returns HTTP 401 with\n  {\"statusCode\":401,\"message\":\"UnauthorizedException\"}. The auth mechanism is\n  therefore real but undocumented in the machine-readable contract. This profile\n  records what was observed live on 2026-07-19 rather than asserting a scheme the\n  provider has not published. derive-authentication.py produced no profile for\n  this provider (0 schemes) — this file is the probed supplement.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  documented_in_spec: false\n  auth_required: true\nschemes: []\nobserved:\n  enforcement: gateway\n  note: >-\n    The 401 is returned before routing — unknown paths (/v1/nope) and unsupported\n    methods (DELETE)\
  \ also return 401 rather than 404/405, indicating a global\n    authentication guard ahead of the router.\n  challenge_header: null\n  www_authenticate: absent\n  error_envelope:\n    statusCode: 401\n    message: UnauthorizedException\n  probes:\n    - {path: /v1/support-schemes, method: GET, status: 401}\n    - {path: /v1/applications, method: GET, status: 401}\n    - {path: /v1/webhooks, method: GET, status: 401}\n    - {path: /v1/support-schemes, method: GET, header: 'Authorization: Bearer <invalid>', status: 401}\n    - {path: /v1/support-schemes, method: GET, header: 'x-api-key: <invalid>', status: 401}\n    - {path: /docs, method: GET, status: 200, note: Swagger UI is public}\ntenancy:\n  model: organisation\n  evidence: >-\n    The GET /v1/support-schemes operation description reads \"Retrieves all\n    available support schemes for the authenticated organisation\", so credentials\n    are scoped to a partner organisation rather than an end user.\ngaps:\n  - securitySchemes absent\
  \ from the OpenAPI; agents cannot discover how to authenticate.\n  - No WWW-Authenticate challenge on 401.\n  - No public authentication documentation page found on lightningreach.org.\n  - Credentials appear to be issued via partner onboarding (contact hello@lightningreach.org).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightning-social-ventures/refs/heads/main/authentication/lightning-social-ventures-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Financial Inclusion
- Grants
- Social Impact
- Nonprofit
- Housing
- Government
- Welfare Benefits
- United Kingdom
---
