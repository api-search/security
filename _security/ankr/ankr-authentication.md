---
api_key_in:
- query
api_specs:
- filename: ankr-rpc-service-openapi.yml
  format: yaml
  label: Ankr RPC Service (Node API)
  slug: ankr-rpc-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-rpc-service-openapi.yml
- filename: ankr-advanced-api-openapi.yml
  format: yaml
  label: Ankr Advanced API
  slug: ankr-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-advanced-api-openapi.yml
- filename: ankr-staking-api-openapi.yml
  format: yaml
  label: Ankr Liquid Staking API
  slug: ankr-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-staking-api-openapi.yml
- filename: ankr-automation-api-openapi.yml
  format: yaml
  label: Ankr Contract Automation API
  slug: ankr-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-automation-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ankr Authentication
name_suffix: Authentication
oauth_flows: []
overview: ankr secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ankr
provider_slug: ankr
scheme_count: 2
schemes:
- description: Premium Plan API key passed as the trailing path segment.
  in: query
  name: ApiKeyAuth
  parameter: API_KEY
  sources:
  - openapi/ankr-advanced-api-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ankr-automation-api-openapi.yml
  type: http
slug: ankr-authentication
source_filename: ankr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ankr-advanced-api-openapi.yml, openapi/ankr-automation-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: API_KEY\n  description: Premium Plan API key passed as the trailing path segment.\n  sources:\n  - openapi/ankr-advanced-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ankr-automation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/authentication/ankr-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
