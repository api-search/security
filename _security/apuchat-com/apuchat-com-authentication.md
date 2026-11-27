---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apuchat-com-channels-api-openapi.yml
  format: yaml
  label: Apuchat Channels API
  slug: apuchat-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-channels-api-openapi.yml
- filename: apuchat-com-healthz-api-openapi.yml
  format: yaml
  label: Apuchat Healthz API
  slug: apuchat-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-healthz-api-openapi.yml
- filename: apuchat-com-info-api-openapi.yml
  format: yaml
  label: Apuchat Info API
  slug: apuchat-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-info-api-openapi.yml
- filename: apuchat-com-stats-api-openapi.yml
  format: yaml
  label: Apuchat Stats API
  slug: apuchat-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-stats-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Apuchat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apuchat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apuchat
provider_slug: apuchat-com
scheme_count: 1
schemes:
- description: Channel token. Get it from the operator who created the channel, or by calling POST /api/channels first.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apuchat-com-openapi.json
  type: http
slug: apuchat-com-authentication
source_filename: apuchat-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/apuchat-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Channel token. Get it from the operator who created the channel, or by calling\n    POST /api/channels first.\n  sources:\n  - openapi/apuchat-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/apuchat-com/authentication/apuchat-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Communications
- Multi-Agent
- MCP
- Chat
---
