---
api_key_in: []
api_specs:
- filename: jobox-ai-kili-openapi.json
  format: json
  label: Jobox Kili API
  slug: kili
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobox-ai/refs/heads/main/openapi/jobox-ai-kili-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Jobox Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: JOBOX.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: JOBOX.ai
provider_slug: jobox-ai
scheme_count: 2
schemes:
- declared_in_spec: false
  evidence: Carried as an explicit header parameter on 52 of 110 operations in openapi/jobox-ai-kili-openapi.json (also spelled user-id / User-id on 16 more).
  in: header
  name: User-Id
  note: A caller-identity header, not by itself proof of a bearer credential; the transport credential is not described anywhere Jobox publishes.
  type: apiKey
- declared_in_spec: false
  evidence: GET https://api.jobox.ai/Kili/occupations -> HTTP 401 {"title":"Unauthorized","message":"You cannot access this resource","debug_id":"dbg_..."} on 2026-08-23.
  in: unknown
  name: undocumented
  note: The mechanism that satisfies this 401 is not published. Onboarding is sales-gated.
  type: unknown
slug: jobox-ai-authentication
source_filename: jobox-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://api.jobox.ai/Kili/occupations (HTTP 401) + openapi/jobox-ai-kili-openapi.json\nname: Jobox Kili API authentication\nnote: The published contract declares NO securityDefinitions at all — a gap in the auto-generated spec,\n  not evidence the API is open. The live production API rejects anonymous requests with HTTP 401, so a\n  credential is required and is simply undocumented in the contract. Jobox publishes no public developer\n  authentication page; the marketplace product is sold through \"Request a demo\" / \"Contact Sales\".\nsecurity_schemes_declared: 0\nschemes:\n- name: User-Id\n  type: apiKey\n  in: header\n  declared_in_spec: false\n  evidence: Carried as an explicit header parameter on 52 of 110 operations in openapi/jobox-ai-kili-openapi.json\n    (also spelled user-id / User-id on 16 more).\n  note: A caller-identity header, not by itself proof of a bearer credential; the transport credential\n    is not described\
  \ anywhere Jobox publishes.\n- name: undocumented\n  type: unknown\n  in: unknown\n  declared_in_spec: false\n  evidence: GET https://api.jobox.ai/Kili/occupations -> HTTP 401 {\"title\":\"Unauthorized\",\"message\":\"You\n    cannot access this resource\",\"debug_id\":\"dbg_...\"} on 2026-08-23.\n  note: The mechanism that satisfies this 401 is not published. Onboarding is sales-gated.\nother_headers_observed:\n- name: User-Id\n  operations: 52\n- name: user-id\n  operations: 15\n- name: Timezone\n  operations: 8\n- name: Version\n  operations: 4\n- name: timezone\n  operations: 2\n- name: version\n  operations: 1\n- name: platform\n  operations: 1\n- name: User-id\n  operations: 1\n- name: password\n  operations: 1\noauth2: false\nopenid_connect: false\nmutual_tls: false\ndocs: null\ngaps:\n- No securityDefinitions in the contract.\n- No public authentication documentation.\n- No published key-issuance or onboarding self-service flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobox-ai/refs/heads/main/authentication/jobox-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Home Services
- Field Service Management
- Marketplace
- Payments
- Fintech
- Dispatching
- Skilled Trades
- KYC
- Wallet
---
