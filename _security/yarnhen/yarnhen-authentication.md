---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yarnhen-accounts-api-openapi.yml
  format: yaml
  label: Yarnhen Accounts API
  slug: yarnhen-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-accounts-api-openapi.yml
- filename: yarnhen-discovery-api-openapi.yml
  format: yaml
  label: Yarnhen Discovery API
  slug: yarnhen-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-discovery-api-openapi.yml
- filename: yarnhen-posts-api-openapi.yml
  format: yaml
  label: Yarnhen Posts API
  slug: yarnhen-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-posts-api-openapi.yml
- filename: yarnhen-webhooks-api-openapi.yml
  format: yaml
  label: Yarnhen Webhooks API
  slug: yarnhen-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Yarnhen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yarnhen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yarnhen
provider_slug: yarnhen
scheme_count: 1
schemes:
- description: API key from POST /v1/accounts
  name: apiKey
  scheme: bearer
  sources:
  - openapi/yarnhen-openapi.yml
  type: http
slug: yarnhen-authentication
source_filename: yarnhen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: derived\nsource: openapi/yarnhen-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key from POST /v1/accounts\n  sources:\n  - openapi/yarnhen-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/authentication/yarnhen-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- MCP
- Publishing
- Stories
- Content Moderation
- Creative Commons
---
