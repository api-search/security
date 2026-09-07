---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: corva-ai-platform-api-openapi.yml
  format: yaml
  label: Corva Platform API
  slug: corva-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corva-ai/refs/heads/main/openapi/corva-ai-platform-api-openapi.yml
- filename: corva-ai-data-api-openapi.yml
  format: yaml
  label: Corva Data API
  slug: corva-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corva-ai/refs/heads/main/openapi/corva-ai-data-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Corva Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corva AI secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Corva AI
provider_slug: corva-ai
scheme_count: 3
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/corva-ai-data-api-openapi.yml
  type: http
- in: header
  name: APIKeyHeader
  parameter: Authorization
  sources:
  - openapi/corva-ai-data-api-openapi.yml
  type: apiKey
- in: header
  name: api_key
  parameter: authorization
  sources:
  - openapi/corva-ai-platform-api-openapi.yml
  type: apiKey
slug: corva-ai-authentication
source_filename: corva-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/corva-ai-data-api-openapi.yml, openapi/corva-ai-platform-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/corva-ai-data-api-openapi.yml\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/corva-ai-data-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/corva-ai-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corva-ai/refs/heads/main/authentication/corva-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Analytics
- Artificial Intelligence
- Completions
- Custom Apps
- Data API
- Dev Center
- Dev Center Apps
- Drilling
- Energy
- Geoscience
- Oil and Gas
- Platform API
- Predictive Drilling
- Python SDK
- Real-Time
- Real-Time Analytics
- Sensor Data
- Sustainability
- Time Series
- WITS
- Well Data
---
