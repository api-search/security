---
api_key_in:
- header
api_specs:
- filename: hourone-openapi-original.json
  format: json
  label: HourOne (MakeReals) Video Generation API
  slug: hourone-makereals-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourone/refs/heads/main/openapi/hourone-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hourone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hourone secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hourone
provider_slug: hourone
scheme_count: 2
schemes:
- in: header
  name: APIKeyHeader
  parameter: api-key
  sources:
  - openapi/hourone-openapi-original.json
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/hourone-openapi-original.json
  type: http
slug: hourone-authentication
source_filename: hourone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hourone-openapi-original.json\ndocs: https://hourone.gitbook.io/api-docs/get-your-api-keys\nnotes: >-\n  Primary auth is a single API key sent in the `api-key` request header (docs:\n  \"Get Your API Keys\"). Only one key is active at a time; generating a new key\n  revokes the previous one; keys are encrypted and cannot be retrieved after\n  creation. Keys are managed via GET/POST/DELETE /keys. The OpenAPI also declares\n  an HTTP bearer scheme. No OAuth2 / OIDC scopes exist, so no scopes/ artifact.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/hourone-openapi-original.json\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hourone-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hourone/refs/heads/main/authentication/hourone-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Generative AI
- AI Avatars
- Text to Speech
- Media
- Content Creation
- Webhooks
---
