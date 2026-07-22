---
api_key_in: []
api_specs:
- filename: usenarrative-sports-openapi-original.json
  format: json
  label: Narrative Sports API
  slug: narrative-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usenarrative/refs/heads/main/openapi/usenarrative-sports-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Usenarrative Authentication
name_suffix: Authentication
oauth_flows: []
overview: Narrative Sports secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Narrative Sports
provider_slug: usenarrative
scheme_count: 1
schemes:
- details:
    display: keys shown truncated in the dashboard (e.g. sk-nr-a1b2****)
    failure_modes:
      '401': missing or invalid API key (detail envelope)
      '403': account not enabled for task creation (no concurrent task limit configured)
    header: 'Authorization: Bearer <API_KEY>'
    key_format: sk-nr-<32 hex characters>
    key_management: https://app.narrative-sports.com/api-dashboard
    unauthenticated_endpoints:
    - GET /v1/health
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/usenarrative-sports-openapi-original.json
  type: http
slug: usenarrative-authentication
source_filename: usenarrative-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/usenarrative-sports-openapi-original.json\ndocs: https://docs.narrative-sports.com/authentication\nsummary:\n  types:\n  - http\n  scheme: bearer\n  credential: static API key sent as a Bearer token\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/usenarrative-sports-openapi-original.json\n  details:\n    header: 'Authorization: Bearer <API_KEY>'\n    key_format: sk-nr-<32 hex characters>\n    key_management: https://app.narrative-sports.com/api-dashboard\n    display: keys shown truncated in the dashboard (e.g. sk-nr-a1b2****)\n    unauthenticated_endpoints:\n    - GET /v1/health\n    failure_modes:\n      '401': 'missing or invalid API key (detail envelope)'\n      '403': 'account not enabled for task creation (no concurrent task limit configured)'\nnotes: No OAuth2/OIDC surface — a single static API-key-as-bearer scheme covers\n  the whole API. Keys are created and rotated in\
  \ the app dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usenarrative/refs/heads/main/authentication/usenarrative-authentication.yml
summary_line: http · 1 scheme
tags:
- Sports
- Video
- Artificial Intelligence
- Highlights
- Broadcasting
- Media
- Sports Technology
---
