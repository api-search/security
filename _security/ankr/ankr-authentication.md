---
api_key_in:
- query
api_specs:
- filename: ankr-evm-api-openapi.yml
  format: yaml
  label: ankr EVM API
  slug: ankr-evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-evm-api-openapi.yml
- filename: ankr-metrics-api-openapi.yml
  format: yaml
  label: ankr Metrics API
  slug: ankr-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-metrics-api-openapi.yml
- filename: ankr-nft-api-openapi.yml
  format: yaml
  label: ankr NFT API
  slug: ankr-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-nft-api-openapi.yml
- filename: ankr-query-api-openapi.yml
  format: yaml
  label: ankr Query API
  slug: ankr-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-query-api-openapi.yml
- filename: ankr-ratio-api-openapi.yml
  format: yaml
  label: ankr Ratio API
  slug: ankr-ratio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-ratio-api-openapi.yml
- filename: ankr-tasks-api-openapi.yml
  format: yaml
  label: ankr Tasks API
  slug: ankr-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-tasks-api-openapi.yml
- filename: ankr-token-api-openapi.yml
  format: yaml
  label: ankr Token API
  slug: ankr-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-token-api-openapi.yml
- filename: ankr-validators-api-openapi.yml
  format: yaml
  label: ankr Validators API
  slug: ankr-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-validators-api-openapi.yml
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
