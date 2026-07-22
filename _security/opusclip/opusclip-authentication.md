---
api_key_in: []
api_specs:
- filename: opusclip-openapi-original.json
  format: json
  label: OpusClip Clip API
  slug: opusclip-clip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Opusclip Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpusClip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpusClip
provider_slug: opusclip
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/opusclip-openapi-original.json
  type: http
slug: opusclip-authentication
source_filename: opusclip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/opusclip-openapi-original.json\ndocs: https://help.opus.pro/api-reference/overview\nsummary:\n  types:\n  - http\n  scheme: HTTP Bearer token; the API key is a JWT-format value passed as a Bearer token\n  header: 'Authorization: Bearer <API_KEY>'\n  org_header: 'x-opus-org-id: <ORG_ID> (required on some endpoints)'\n  key_source: OpusClip dashboard (https://clip.opus.pro/dashboard); Enterprise/Pro(Beta)/Max plans\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/opusclip-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/authentication/opusclip-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Video
- AI
- Video Editing
- Short-Form Video
- Social Media
- Content Creation
- MCP
- Developer API
---
