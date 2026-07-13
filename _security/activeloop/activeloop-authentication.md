---
api_key_in: []
api_specs:
- filename: activeloop-openapi.yml
  format: yaml
  label: Deep Lake SDK (Python)
  slug: deep-lake-python-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/openapi/activeloop-openapi.yml
- filename: activeloop-openapi.yml
  format: yaml
  label: Tensor Query Language (TQL)
  slug: tensor-query-language
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/openapi/activeloop-openapi.yml
- filename: activeloop-openapi.yml
  format: yaml
  label: Deep Lake Vector Store
  slug: vector-store
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/openapi/activeloop-openapi.yml
- filename: activeloop-openapi.yml
  format: yaml
  label: Activeloop Managed Database REST API
  slug: managed-database-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/openapi/activeloop-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Activeloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Activeloop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Activeloop
provider_slug: activeloop
scheme_count: 1
schemes:
- description: 'Activeloop API token passed as `Authorization: Bearer {ACTIVELOOP_TOKEN}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/activeloop-openapi.yml
  type: http
slug: activeloop-authentication
source_filename: activeloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/activeloop-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Activeloop API token passed as `Authorization: Bearer {ACTIVELOOP_TOKEN}`.'\n  sources:\n  - openapi/activeloop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/authentication/activeloop-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Vector Store
- Data Lake
- Multimodal
- Deep Learning
- Python SDK
---
