---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Accuracite Authentication
name_suffix: Authentication
oauth_flows: []
overview: AccuraCite declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AccuraCite
provider_slug: accuracite
scheme_count: 1
schemes:
- applies_to:
  - POST /api/v1/verify
  - POST /api/v1/generate
  description: 'All endpoints require an API key passed in the X-API-Key header. Key issuance is tied to a paid plan: the docs and the pricing FAQ both state that API access requires the Pro or Bulk Verification plan, and the free plan cannot call the API.'
  in: header
  key_prefix: null
  key_prefix_note: The provider does not document a key prefix or key format.
  name: apiKeyHeader
  parameter: X-API-Key
  required: true
  type: apiKey
slug: accuracite-authentication
source_filename: accuracite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: searched\nsource: https://accuracite.com/api-docs\ndocs: https://accuracite.com/api-docs\nnote: >-\n  AccuraCite publishes no OpenAPI, so this profile was read from the published API\n  reference and confirmed against a live unauthenticated request. There are no\n  OAuth, OIDC or mTLS surfaces — a single API key header is the whole auth model.\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  required: true\n  applies_to:\n  - POST /api/v1/verify\n  - POST /api/v1/generate\n  description: >-\n    All endpoints require an API key passed in the X-API-Key header. Key issuance is\n    tied to a paid plan: the docs and the pricing FAQ both state that API access\n    requires the Pro or Bulk Verification plan, and the free plan cannot call the API.\n  key_prefix: null\n  key_prefix_note: The provider does not document a key prefix or key format.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nentitlement:\n\
  \  model: plan-gated\n  free_tier_api_access: false\n  paid_plans_with_api_access:\n  - Pro\n  - Bulk Verification\n  source: https://accuracite.com/pricing\nobserved:\n- probe: POST https://accuracite.com/api/v1/verify with no X-API-Key\n  date: '2026-08-31'\n  http_status: 401\n  content_type: application/json\n  body: '{\"error\":\"Unauthorized. Please provide a valid X-API-Key header.\"}'\nfailure_modes:\n- status: 401\n  meaning: Missing or invalid X-API-Key.\n- status: 403\n  meaning: Key is valid but the account is not on a plan that includes API access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accuracite/refs/heads/main/authentication/accuracite-authentication.yml
summary_line: 1 scheme
tags:
- Citations
- Research
- Bibliography
- Academic
- Verification
- AI Safety
---
