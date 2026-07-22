---
api_key_in:
- header
- query
api_specs:
- filename: sentio-openapi.yml
  format: yaml
  label: Sentio API
  slug: sentio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sentio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sentio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sentio
provider_slug: sentio
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeaderAuth
  parameter: api-key
  sources:
  - openapi/sentio-openapi.yml
  type: apiKey
- in: query
  name: ApiKeyQueryAuth
  parameter: api-key
  sources:
  - openapi/sentio-openapi.yml
  type: apiKey
slug: sentio-authentication
source_filename: sentio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sentio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeaderAuth\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/sentio-openapi.yml\n- name: ApiKeyQueryAuth\n  type: apiKey\n  in: query\n  parameter: api-key\n  sources:\n  - openapi/sentio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/authentication/sentio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Web3
- Blockchain
- Observability
- Analytics
- Data
- Indexing
- Monitoring
- Developer Tools
- Crypto
- API
---
