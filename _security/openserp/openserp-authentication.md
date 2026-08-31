---
api_key_in:
- header
api_specs:
- filename: openserp-docs-api-openapi.yml
  format: yaml
  label: OpenSERP Docs API
  slug: openserp-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openserp/refs/heads/main/openapi/openserp-docs-api-openapi.yml
- filename: openserp-health-api-openapi.yml
  format: yaml
  label: OpenSERP Health API
  slug: openserp-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openserp/refs/heads/main/openapi/openserp-health-api-openapi.yml
- filename: openserp-mega-api-openapi.yml
  format: yaml
  label: OpenSERP Mega API
  slug: openserp-mega-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openserp/refs/heads/main/openapi/openserp-mega-api-openapi.yml
- filename: openserp-search-api-openapi.yml
  format: yaml
  label: OpenSERP Search API
  slug: openserp-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openserp/refs/heads/main/openapi/openserp-search-api-openapi.yml
- filename: openserp-stats-api-openapi.yml
  format: yaml
  label: OpenSERP Stats API
  slug: openserp-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openserp/refs/heads/main/openapi/openserp-stats-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Openserp Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenSERP secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenSERP
provider_slug: openserp
scheme_count: 2
schemes:
- applies_to: https://api.openserp.org
  description: OpenSERP Cloud API key issued from the dashboard API keys page. The full secret is shown once at creation; a safe-to-log prefix is retained for identification.
  format: Bearer <api key>
  header: Authorization
  in: header
  name: cloudBearerToken
  note: Keys are account-wide. The documentation describes no per-key scopes, permissions or restrictions, so there is no scope surface to capture (scopes/ is intentionally absent).
  scheme: bearer
  scopes: none
  sources:
  - https://openserp.org/docs/cloud-authentication/
  token_prefix: osk_live_
  type: http
- applies_to: http://localhost:7000
  description: 'The self-hosted OpenSERP server requires no credentials. The OpenAPI declares an empty top-level `security: []` and no `components.securitySchemes`.'
  name: none
  sources:
  - openapi/openserp-oss-openapi.yml
  type: none
slug: openserp-authentication
source_filename: openserp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: searched\nsource: https://openserp.org/docs/cloud-authentication/\ndocs: https://openserp.org/docs/cloud-authentication/\nnote: derive-authentication.py returned no schemes because the published OSS OpenAPI declares no\n  `securitySchemes` — the self-hosted server is deliberately unauthenticated. The Cloud auth model\n  below was read from the provider's documentation and confirmed against live 401 responses.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: cloudBearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Bearer <api key>\"\n  token_prefix: osk_live_\n  applies_to: https://api.openserp.org\n  sources: [https://openserp.org/docs/cloud-authentication/]\n  description: OpenSERP Cloud API key issued from the dashboard API keys page. The full secret is\n    shown once at creation; a safe-to-log\
  \ prefix is retained for identification.\n  scopes: none\n  note: Keys are account-wide. The documentation describes no per-key scopes, permissions or\n    restrictions, so there is no scope surface to capture (scopes/ is intentionally absent).\n- name: none\n  type: none\n  applies_to: http://localhost:7000\n  sources: [openapi/openserp-oss-openapi.yml]\n  description: 'The self-hosted OpenSERP server requires no credentials. The OpenAPI declares an\n    empty top-level `security: []` and no `components.securitySchemes`.'\nkey_management:\n  issuance: https://openserp.org/dashboard/keys\n  visibility: full secret shown once at creation\n  environment_variable: OPENSERP_API_KEY\n  rotation:\n    documented: true\n    procedure:\n    - Create a new key in the dashboard.\n    - Update the OPENSERP_API_KEY environment variable.\n    - Deploy and verify with client.me() (GET /v1/me).\n    - Revoke the old key.\n    note: Overlapping validity is explicitly recommended so in-flight requests\
  \ do not fail.\n  revocation: dashboard\n  validation_endpoint:\n    operation: GET /v1/me\n    cost: 0 credits\n    description: Validates a key and returns account details and credit balance. Documented as the\n      deployment smoke test.\n  test_vs_live: single live key class (`osk_live_`). No separate test/sandbox key prefix is\n    documented.\nfailure_modes:\n- status: 401\n  error: unauthorized\n  body: '{\"error\": \"unauthorized\", \"code\": 401, \"message\": \"missing or invalid API key\"}'\n  causes: [missing key, wrong key, revoked key]\n  retryable: false\nx-evidence:\n  fetched: '2026-08-10'\n  checks:\n  - url: https://openserp.org/docs/cloud-authentication/\n    http_status: 200\n  - url: https://api.openserp.org/v1/me\n    http_status: 401\n    note: Anonymous request returned the documented envelope verbatim -\n      {\"error\":\"unauthorized\",\"code\":401,\"message\":\"missing or invalid api key\"}\n  - url: https://api.openserp.org/v1/pricing\n    http_status: 200\n\
  \    note: The one Cloud operation that answers anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openserp/refs/heads/main/authentication/openserp-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Search
- SERP
- Search API
- Web Scraping
- Content Extraction
- AI Grounding
- Rank Tracking
- Open-Source
- Developer Tools
---
