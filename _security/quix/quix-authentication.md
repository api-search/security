---
api_key_in: []
api_specs:
- filename: quix-openapi.yml
  format: yaml
  label: Quix Streaming Writer API
  slug: streaming-writer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
- filename: quix-asyncapi.yml
  format: yaml
  label: Quix Streaming Reader API (Real-time)
  slug: streaming-reader-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/asyncapi/quix-asyncapi.yml
- filename: quix-openapi.yml
  format: yaml
  label: Quix Portal API (Management)
  slug: portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
- filename: quix-openapi.yml
  format: yaml
  label: Quix Topics & Deployments API
  slug: topics-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quix
provider_slug: quix
scheme_count: 1
schemes:
- bearerFormat: PAT
  description: 'Quix Personal Access Token (PAT) presented as `Authorization: Bearer <PAT>`. Generate from the Quix portal under your profile > Personal Access Tokens, or Settings > APIs and tokens.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/quix-openapi.yml
  type: http
slug: quix-authentication
source_filename: quix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quix-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  description: 'Quix Personal Access Token (PAT) presented as `Authorization: Bearer <PAT>`.\n    Generate from the Quix portal under your profile > Personal Access Tokens, or Settings >\n    APIs and tokens.'\n  sources:\n  - openapi/quix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/authentication/quix-authentication.yml
summary_line: http · 1 scheme
tags:
- Stream Processing
- Real Time
- Kafka
- Python
- Streaming Data
---
