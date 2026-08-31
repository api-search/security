---
api_key_in:
- query
api_specs:
- filename: insightera-classification-api-openapi.yml
  format: yaml
  label: InsightEra Classification API
  slug: insightera-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightera/refs/heads/main/openapi/insightera-classification-api-openapi.yml
- filename: insightera-nlp-api-openapi.yml
  format: yaml
  label: InsightEra Nlp API
  slug: insightera-nlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightera/refs/heads/main/openapi/insightera-nlp-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Insightera Authentication
name_suffix: Authentication
oauth_flows: []
overview: InsightEra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InsightEra
provider_slug: insightera
scheme_count: 1
schemes:
- applies_to_operations: 23
  declared_as_security_scheme: false
  description: Per-account service token issued by InsightEra. Passed as `?token=<value>` on every request. The public API reference pre-populates a shared demo token in the Swagger UI "try it" console; that token is quota-limited and returns HTTP 403 on the live service.
  in: query
  name: token
  parameter: token
  required: true
  sources:
  - openapi/insightera-nlp-platform-openapi.yml
  type: apiKey
slug: insightera-authentication
source_filename: insightera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/insightera-nlp-platform-openapi.yml\ndocs: https://nlp.insightera.co.th/docs/v1.0/\nnote: >-\n  The published Swagger 2.0 document declares no `securityDefinitions` block. Authentication is\n  instead carried as an ordinary required request parameter — a `token` string in the query\n  string — repeated on all 23 operations. This artifact is derived from those parameter\n  declarations plus an observed live response, because the spec's own security machinery is\n  unused. That is the single largest contract-quality gap on this API: an agent or code\n  generator reading the spec sees no security scheme at all and will emit an unauthenticated\n  client.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  schemes_declared_in_spec: 0\nschemes:\n- name: token\n  type: apiKey\n  in: query\n  parameter: token\n  required: true\n  declared_as_security_scheme:\
  \ false\n  applies_to_operations: 23\n  description: >-\n    Per-account service token issued by InsightEra. Passed as `?token=<value>` on every request.\n    The public API reference pre-populates a shared demo token in the Swagger UI \"try it\"\n    console; that token is quota-limited and returns HTTP 403 on the live service.\n  sources:\n  - openapi/insightera-nlp-platform-openapi.yml\nobserved:\n  probed: '2026-08-13'\n  missing_or_invalid_token:\n    http_status: 400\n    body: '{\"message\":\"Invalid session token\"}'\n    note: >-\n      The spec documents 401 Unauthorized for auth failure; the live service answers HTTP 400\n      with a flat `message` envelope. Spec and runtime disagree.\n  quota_exhausted_token:\n    http_status: 403\n    body: '{\"message\":\"This token has no quota allowed on this service\"}'\n    note: Per-token, per-service quota enforcement observed on the published demo token.\nissuance:\n  self_service: false\n  process: Contact InsightEra sales/support;\
  \ no public signup or key-issuance page was found.\n  contact: dev@insightera.co.th\n  source: openapi/_original/insightera-nlp-platform-openapi.json (info.contact)\ngaps:\n- No securityDefinitions in the OpenAPI/Swagger document.\n- Credential travels in the query string, so it lands in server logs, proxy logs and browser\n  history; a header or Authorization bearer scheme would be the standard remedy.\n- No OAuth 2.0, no OpenID Connect, no scopes, no key rotation or expiry policy published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insightera/refs/heads/main/authentication/insightera-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketing Technology
- Social Listening
- Data Analytics
- Customer Data Platform
- CRM
- Chatbots
- Social Media Management
- Natural Language Processing
- Artificial Intelligence
---
