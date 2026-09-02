---
api_key_in: []
api_specs:
- filename: dreamthreads-dream-interpretation-api-openapi.yml
  format: yaml
  label: DreamThreads Dream interpretation API
  slug: dreamthreads-dream-interpretation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamthreads/refs/heads/main/openapi/dreamthreads-dream-interpretation-api-openapi.yml
- filename: dreamthreads-dream-parsing-api-openapi.yml
  format: yaml
  label: DreamThreads Dream parsing API
  slug: dreamthreads-dream-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamthreads/refs/heads/main/openapi/dreamthreads-dream-parsing-api-openapi.yml
auth_types:
- http
- none
description: ''
kind: authentication
layout: security
method: searched
name: Dreamthreads Authentication
name_suffix: Authentication
oauth_flows: []
overview: DreamThreads secures its APIs with http and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DreamThreads
provider_slug: dreamthreads
scheme_count: 2
schemes:
- applies_to:
  - interpretDream
  - parseDream
  bearerFormat: DreamThreads partner API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dreamthreads-dreamgraph-openapi.yml
  type: http
- applies_to:
  - getDreamGraphHealth
  - parseDreamPublicly
  - mcp:parse_dream
  - mcp:search_dream_concepts
  name: none
  note: 'Declared explicitly in the OpenAPI as an empty operation-level `security: []` override on /health and /public/parse, and confirmed anonymously against the live MCP server.'
  type: none
slug: dreamthreads-authentication
source_filename: dreamthreads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/dreamthreads-dreamgraph-openapi.yml\ndocs:\n  - https://mydreamthreads.xyz/dream-interpretation-api#request-access\n  - https://mydreamthreads.xyz/.well-known/api-onboarding\nsummary:\n  types:\n  - http\n  - none\n  http_schemes:\n  - bearer\n  keyless_surfaces: 3\n  reviewed_surfaces: 2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: DreamThreads partner API key\n  applies_to:\n  - interpretDream\n  - parseDream\n  sources:\n  - openapi/dreamthreads-dreamgraph-openapi.yml\n- name: none\n  type: none\n  applies_to:\n  - getDreamGraphHealth\n  - parseDreamPublicly\n  - mcp:parse_dream\n  - mcp:search_dream_concepts\n  note: >-\n    Declared explicitly in the OpenAPI as an empty operation-level `security: []` override on\n    /health and /public/parse, and confirmed anonymously against the live MCP server.\naccess_model:\n  keyless:\n    - surface: POST /api/v1/dreamgraph/public/parse\n\
  \      auth: none\n      note: CORS-enabled, 12/min and 100/day per client, dream text not stored.\n    - surface: GET /api/v1/dreamgraph/health\n      auth: none\n    - surface: https://mydreamthreads.xyz/mcp\n      auth: none\n      note: Streamable HTTP MCP server, anonymous tools/list confirmed 2026-08-14.\n  reviewed:\n    - surface: POST /api/v1/dreamgraph/interpret\n      auth: bearer\n    - surface: POST /api/v1/dreamgraph/parse\n      auth: bearer\ncredential_issuance:\n  mechanism: human review\n  request_url: https://mydreamthreads.xyz/dream-interpretation-api#request-access\n  issued_by: DreamThreads after partner review\n  automatic_keys: false\n  note: >-\n    The provider states plainly that there are no automatic keys — a partner integration form is\n    reviewed by a human before a bearer key is issued.\nkey_handling:\n  storage: keys hashed at rest\n  binding: tied to a partner account and restricted by origin\n  controls: [rate-limited, pausable, rotatable]\n  client_side_use:\
  \ forbidden — partner keys must stay in a server-side secret manager\n  rotation_contact: rahim@mydreamthreads.xyz\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  model: endpoint\n  note: >-\n    No OAuth scope surface exists. Authorization is per-endpoint: keyless operations are open, and a\n    partner key authorizes the reviewed endpoints enabled for that integration. scopes/ is\n    intentionally not emitted.\nembed_tokens:\n  mechanism: short-lived, origin-bound token issued to an approved domain for the hosted embed\n  note: Keeps the partner key out of browser code. See components/dreamthreads-components.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamthreads/refs/heads/main/authentication/dreamthreads-authentication.yml
summary_line: http/none · 2 schemes
tags:
- dream analysis
- Dream interpretation
- Natural Language Processing
- structured parsing
- AI Agents
- MCP Server
- OpenAPI
- wellness / sleep
- research tooling
---
