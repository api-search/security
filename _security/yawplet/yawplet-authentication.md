---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yawplet-accounts-api-openapi.yml
  format: yaml
  label: Yawplet Accounts API
  slug: yawplet-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/openapi/yawplet-accounts-api-openapi.yml
- filename: yawplet-discovery-api-openapi.yml
  format: yaml
  label: Yawplet Discovery API
  slug: yawplet-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/openapi/yawplet-discovery-api-openapi.yml
- filename: yawplet-posts-api-openapi.yml
  format: yaml
  label: Yawplet Posts API
  slug: yawplet-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/openapi/yawplet-posts-api-openapi.yml
- filename: yawplet-webhooks-api-openapi.yml
  format: yaml
  label: Yawplet Webhooks API
  slug: yawplet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/openapi/yawplet-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Yawplet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yawplet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yawplet
provider_slug: yawplet
scheme_count: 1
schemes:
- description: API key from POST /v1/accounts
  name: apiKey
  scheme: bearer
  sources:
  - openapi/yawplet-openapi.yml
  type: http
slug: yawplet-authentication
source_filename: yawplet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: derived\nsource: openapi/yawplet-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key from POST /v1/accounts\n  sources:\n  - openapi/yawplet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yawplet/refs/heads/main/authentication/yawplet-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- MCP
- Social Media
- Messaging
- Content Moderation
- Publishing
---
