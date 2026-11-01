---
anonymous_access: false
api_key_in: []
api_specs:
- filename: transcript1-com-openapi.json
  format: json
  label: Transcript1 API
  slug: transcript1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcript1-com/openapi/transcript1-com-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Transcript1 Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: transcript1-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: transcript1-com
provider_slug: transcript1-com
scheme_count: 1
schemes:
- bearerFormat: API key or OAuth token
  description: transcript1 API key (t1_...) or OAuth access token (t1o_...).
  docs: https://transcript1.com/docs/sdk#api-key
  scheme: bearer
  type: http
slug: transcript1-com-authentication
source_filename: transcript1-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/transcript1-com-openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"transcript1 API key (t1_...) or OAuth access token (t1o_...).\"\n    bearerFormat: \"API key or OAuth token\"\n    docs: \"https://transcript1.com/docs/sdk#api-key\"\n"
source_yaml_url: https://artifacts.apis.io/transcript1-com/authentication/transcript1-com-authentication.yml
summary_line: 1 scheme
tags:
- Audio
- Video
- Transcription
- API
- MCP
---
