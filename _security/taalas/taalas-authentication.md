---
api_key_in:
- header
api_specs:
- filename: taalas-inference-api-openapi.yml
  format: yaml
  label: Taalas API
  slug: taalas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/openapi/taalas-inference-api-openapi.yml
- filename: taalas-inference-v1-api-openapi.yml
  format: yaml
  label: Taalas API v1 (OpenAI-compatible)
  slug: taalas-api-v1-openai-compatible
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/openapi/taalas-inference-v1-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Taalas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taalas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Taalas
provider_slug: taalas
scheme_count: 1
schemes:
- bearer_format: opaque-api-key
  description: Opaque API key presented as an HTTP bearer credential. Applies to every operation on api.taalas.com except GET /health, which is anonymously reachable.
  header: Authorization
  in: header
  name: bearerApiKey
  scheme: bearer
  sources:
  - probe:https://api.taalas.com/models
  - probe:https://api.taalas.com/v1/models
  - probe:https://api.taalas.com/v1/chat/completions
  type: http
slug: taalas-authentication
source_filename: taalas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://api.taalas.com/openapi.json\ndocs: https://api.taalas.com/docs\nnote: >-\n  Neither published Taalas OpenAPI declares components.securitySchemes, so the auth profile below was\n  established by live probing api.taalas.com (2026-08-02) rather than derived from the spec. The\n  probe is unambiguous: an anonymous request returns {\"detail\":\"Unauthorized\"} while a request\n  carrying Authorization: Bearer <value> returns {\"detail\":\"Unauthorized: Invalid API Key\"} — the\n  server distinguishes \"no credential\" from \"bad API key\", and only the Authorization header does so.\n  X-API-Key, api-key and X-Api-Token were probed and produce the generic \"Unauthorized\". Taalas\n  publishes no separate auth documentation page; the API key is issued through the access request\n  form at https://taalas.com/api-request-form/ (applications currently closed) and is the value\n  entered in the \"API Key\" field of the bug report\
  \ form at https://api.taalas.com/bug-report.\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: false\n  multi_tenant: false\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  bearer_format: opaque-api-key\n  in: header\n  header: Authorization\n  description: >-\n    Opaque API key presented as an HTTP bearer credential. Applies to every operation on\n    api.taalas.com except GET /health, which is anonymously reachable.\n  sources:\n  - probe:https://api.taalas.com/models\n  - probe:https://api.taalas.com/v1/models\n  - probe:https://api.taalas.com/v1/chat/completions\nanonymous_operations:\n- operationId: health_health_get\n  path: /health\n  method: get\n  evidence: 'GET https://api.taalas.com/health -> 200 {\"status\":\"healthy\",\"queue_size\":0,\"current_adapter\":\"none\"}'\ncredential_issuance:\n  self_serve: false\n  request_form: https://taalas.com/api-request-form/\n  status: closed\n  statement: >-\n    \"Thank you for your\
  \ interest in our API. Due to overwhelming demand, we are no longer taking\n    applications at this time.\"\n  contact: info@taalas.com\ngaps:\n- The OpenAPI documents declare no securitySchemes and no top-level security requirement, so the\n  machine-readable contract does not describe how to authenticate. Adding an http/bearer scheme\n  would make the published spec self-sufficient for code generation and agent use.\n- No 401 response is declared on any operation in either spec, although 401 is the observed\n  behaviour for every authenticated path.\nx-evidence:\n- fetched: '2026-08-02'\n  url: https://api.taalas.com/models\n  http_status: 401\n  body: '{\"detail\":\"Unauthorized\"}'\n  request_headers: none\n- fetched: '2026-08-02'\n  url: https://api.taalas.com/models\n  http_status: 401\n  body: '{\"detail\":\"Unauthorized: Invalid API Key\"}'\n  request_headers: 'Authorization: Bearer <test value>'\n- fetched: '2026-08-02'\n  url: https://api.taalas.com/health\n  http_status: 200\n\
  \  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/authentication/taalas-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- artificial-intelligence
- ai-inference
- semiconductors
- ai-accelerator
- large-language-models
- llama
- inference-api
- openai-compatible
- hardware
- deep-tech
---
