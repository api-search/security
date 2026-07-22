---
api_key_in:
- header
- query
api_specs:
- filename: zencoder-openapi-original.yml
  format: yaml
  label: Zencoder API
  slug: zencoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zencoder/refs/heads/main/openapi/zencoder-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Zencoder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zencoder secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zencoder
provider_slug: zencoder
scheme_count: 1
schemes:
- description: API key sent on every request in the Zencoder-Api-Key header. Also accepted as an `api_key` query-string parameter (e.g. ?api_key=...).
  in: header
  name: ZencoderApiKey
  parameter_name: Zencoder-Api-Key
  sources:
  - openapi/zencoder-openapi-original.yml
  type: apiKey
slug: zencoder-authentication
source_filename: zencoder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://zencoder.support.brightcove.com/getting-started/getting-api-key.html\ndocs: https://zencoder.support.brightcove.com/getting-started/getting-api-key.html\nnotes: >-\n  The Zencoder v2 OpenAPI models the credential as a required request parameter (ZencoderApiKey) rather\n  than a formal components.securitySchemes entry, so the mechanical auth-derive returns nothing; this\n  profile is authored from the docs. Zencoder authenticates every request with an API key sent in the\n  `Zencoder-Api-Key` HTTP header. The key may alternatively be passed as an `api_key` query-string\n  parameter. There is no OAuth 2.0 / OIDC surface, hence no scopes/ artifact.\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n- name: ZencoderApiKey\n  type: apiKey\n  in: header\n  parameter_name: Zencoder-Api-Key\n  description: >-\n    API key sent on every request in the Zencoder-Api-Key header. Also accepted\
  \ as an `api_key`\n    query-string parameter (e.g. ?api_key=...).\n  sources: [openapi/zencoder-openapi-original.yml]\nkey_types:\n- name: full-access\n  description: Allows any request to the Zencoder API; required to submit jobs and retrieve outputs. Requires a paid plan.\n- name: read-only\n  description: Allows GET requests only (job/output status), no job submission.\n- name: integration-mode\n  description: >-\n    Allows job submission for testing without processing (jobs are accepted but not encoded). Used to\n    build and test integrations before purchasing a paid plan. See sandbox/zencoder-sandbox.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zencoder/refs/heads/main/authentication/zencoder-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Video
- Video Encoding
- Transcoding
- Media
- Streaming
- Video Processing
- Cloud
- Brightcove
- Captions
- DRM
- HLS
---
