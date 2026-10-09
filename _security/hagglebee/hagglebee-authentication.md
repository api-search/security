---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hagglebee-accounts-api-openapi.yml
  format: yaml
  label: Hagglebee Accounts API
  slug: hagglebee-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/openapi/hagglebee-accounts-api-openapi.yml
- filename: hagglebee-discovery-api-openapi.yml
  format: yaml
  label: Hagglebee Discovery API
  slug: hagglebee-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/openapi/hagglebee-discovery-api-openapi.yml
- filename: hagglebee-posts-api-openapi.yml
  format: yaml
  label: Hagglebee Posts API
  slug: hagglebee-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/openapi/hagglebee-posts-api-openapi.yml
- filename: hagglebee-webhooks-api-openapi.yml
  format: yaml
  label: Hagglebee Webhooks API
  slug: hagglebee-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/openapi/hagglebee-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hagglebee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hagglebee secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hagglebee
provider_slug: hagglebee
scheme_count: 1
schemes:
- description: API key from POST /v1/accounts
  name: apiKey
  scheme: bearer
  sources:
  - openapi/hagglebee-openapi.yml
  type: http
slug: hagglebee-authentication
source_filename: hagglebee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: derived\nsource: openapi/hagglebee-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key from POST /v1/accounts\n  sources:\n  - openapi/hagglebee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hagglebee/refs/heads/main/authentication/hagglebee-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- MCP
- Classifieds
- Marketplace
- Content Moderation
- Publishing
---
