---
api_key_in:
- header
api_specs:
- filename: golden-openapi-original.json
  format: json
  label: Golden Public API v2
  slug: golden-public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/openapi/golden-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Golden Authentication
name_suffix: Authentication
oauth_flows: []
overview: Golden secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Golden
provider_slug: golden
scheme_count: 1
schemes:
- description: All requests to the Golden Public API v2 authenticate with an API key passed in the `apikey` request header. Keys are issued from the Golden account/API settings. There is no OAuth or user-delegated flow; the key is a static service credential.
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/golden-openapi-original.json
  type: apiKey
slug: golden-authentication
source_filename: golden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/golden-openapi-original.json\ndocs: https://docs.golden.com\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: >-\n    All requests to the Golden Public API v2 authenticate with an API key\n    passed in the `apikey` request header. Keys are issued from the Golden\n    account/API settings. There is no OAuth or user-delegated flow; the key\n    is a static service credential.\n  sources:\n  - openapi/golden-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/authentication/golden-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Knowledge Graph
- Company Data
- Data
- Entities
- Artificial Intelligence
- Search
- Business Intelligence
---
