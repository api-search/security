---
api_key_in:
- header
api_specs:
- filename: flipside-openapi.yml
  format: yaml
  label: Query Execution (SQL)
  slug: query-execution-sql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
- filename: flipside-openapi.yml
  format: yaml
  label: Query Results
  slug: query-results
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
- filename: flipside-openapi.yml
  format: yaml
  label: Datasets
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Flipside Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flipside Crypto secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flipside Crypto
provider_slug: flipside
scheme_count: 1
schemes:
- description: Flipside Data API key, created in the Flipside account settings.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/flipside-openapi.yml
  type: apiKey
slug: flipside-authentication
source_filename: flipside-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flipside-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Flipside Data API key, created in the Flipside account settings.\n  sources:\n  - openapi/flipside-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/authentication/flipside-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Analytics
- SQL
- Web3
- Data
---
