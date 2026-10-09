---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eventwren-accounts-api-openapi.yml
  format: yaml
  label: Eventwren Accounts API
  slug: eventwren-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-accounts-api-openapi.yml
- filename: eventwren-discovery-api-openapi.yml
  format: yaml
  label: Eventwren Discovery API
  slug: eventwren-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-discovery-api-openapi.yml
- filename: eventwren-posts-api-openapi.yml
  format: yaml
  label: Eventwren Posts API
  slug: eventwren-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-posts-api-openapi.yml
- filename: eventwren-webhooks-api-openapi.yml
  format: yaml
  label: Eventwren Webhooks API
  slug: eventwren-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eventwren Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eventwren secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eventwren
provider_slug: eventwren
scheme_count: 1
schemes:
- description: API key from POST /v1/accounts
  name: apiKey
  scheme: bearer
  sources:
  - openapi/eventwren-openapi.yml
  type: http
slug: eventwren-authentication
source_filename: eventwren-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: derived\nsource: openapi/eventwren-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key from POST /v1/accounts\n  sources:\n  - openapi/eventwren-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/authentication/eventwren-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- MCP
- Event
- Calendar
- Content Moderation
- Publishing
---
