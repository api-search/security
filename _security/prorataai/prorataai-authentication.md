---
api_key_in:
- header
api_specs:
- filename: prorataai-openapi.json
  format: json
  label: Prorata API Service
  slug: prorataai-prorata-api-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/openapi/prorataai-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Prorataai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProRata.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ProRata.ai
provider_slug: prorataai
scheme_count: 1
schemes:
- description: Add your API key with the Bearer prefix (e.g., "Bearer YOUR-API-KEY")
  format: Bearer <api-key>
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/prorataai-openapi.json
  - https://platform.gist.ai/docs/gist-content-api
  type: apiKey
slug: prorataai-authentication
source_filename: prorataai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: openapi/prorataai-openapi.json\ndocs: https://platform.gist.ai/docs/gist-content-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  self_serve: false\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <api-key>'\n  description: Add your API key with the Bearer prefix (e.g., \"Bearer YOUR-API-KEY\")\n  sources:\n  - openapi/prorataai-openapi.json\n  - https://platform.gist.ai/docs/gist-content-api\nkey_issuance:\n  self_serve: false\n  level: Publisher Group\n  process: >-\n    \"API keys are provided during onboarding. Contact us if you need access.\" A single key\n    is issued per Publisher Group and shared by every publication under it; individual\n    publications are identified per-request instead.\n  source: https://platform.gist.ai/docs/gist-content-api\nkey_tiers:\n- name: public key\n\
  - name: secret key\nkey_tier_note: >-\n  POST /v1/summaries and GET /v1/summaries/{summaryId} accept \"a valid API key (public or\n  secret)\". No prefix convention, rotation policy or scope difference between the two\n  tiers is documented anywhere in the hub — a real gap, recorded rather than guessed.\nadditional_identity_headers:\n- name: X-User-ID\n  required: true\n  operation_count: 12\n  operations:\n  - POST /v1/chat\n  - POST /v1/chat/completions\n  - GET /v1/chat/response/{threadId}/{turnId}\n  - GET /v1/chat/citations/{threadId}/{turnId}\n  - GET /v1/chat/attributions/{threadId}/{turnId}\n  - GET /v1/threads\n  - GET /v1/threads/{threadId}\n  - DELETE /v1/threads/{threadId}\n  - GET /v1/questions/recommended\n  - POST /v1/questions/related\n  - GET /v1/publishers\n  - GET /v1/publishers/{id}\n  description: >-\n    Unique identifier for the end user making the request. Declared required: true on 12\n    of the 16 published operations — every one except GET /, GET /v1/health\
  \ and the two\n    /v1/summaries operations. It is a second, mandatory identity input alongside the API\n    key, and it is easy to miss: it is a per-operation parameter, not a security scheme,\n    so a client generated from securitySchemes alone will 400.\nauthorization_model:\n  scopes: false\n  scopes_note: >-\n    No OAuth scopes exist, so no scopes/ artifact is emitted. Authorization is by tenancy,\n    not permission — a key sees only its own publisher group, and POST /v1/summaries\n    additionally validates the target URL's domain against that group with an EXACT match\n    (subdomains are not automatically allowed), returning 403 otherwise.\npublic_operations:\n- GET /v1/health\n- GET /\npublic_note: >-\n  Both are marked \"Public Endpoint: This endpoint is publicly accessible and does not\n  require authentication\" in the contract, and GET https://api.gist.ai/v1/health was\n  confirmed answering anonymously during this pass.\nobserved:\n  url: https://api.gist.ai/v1/publishers\n\
  \  http_status: 401\n  body: '{\"error\":\"Unauthorized\",\"message\":\"Missing or invalid Authorization header\",\"statusCode\":401}'\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prorataai/refs/heads/main/authentication/prorataai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Search
- Content
- Publishing
- Advertising
- Attribution
- Answer Engines
- Generative AI
- Media
- Content Licensing
---
