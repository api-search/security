---
api_key_in:
- header
api_specs:
- filename: gcore-cdn-api-openapi.yml
  format: yaml
  label: Gcore CDN API
  slug: gcore-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-cdn-api-openapi.yml
- filename: gcore-cloud-api-openapi.yml
  format: yaml
  label: Gcore Cloud API
  slug: gcore-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-cloud-api-openapi.yml
- filename: gcore-dns-api-openapi.yml
  format: yaml
  label: Gcore DNS API
  slug: gcore-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-dns-api-openapi.yml
- filename: gcore-fastedge-api-openapi.yml
  format: yaml
  label: Gcore FastEdge API
  slug: gcore-fastedge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-fastedge-api-openapi.yml
- filename: gcore-inference-api-openapi.yml
  format: yaml
  label: Gcore Inference API
  slug: gcore-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-inference-api-openapi.yml
- filename: gcore-storage-api-openapi.yml
  format: yaml
  label: Gcore Storage API
  slug: gcore-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-storage-api-openapi.yml
- filename: gcore-streaming-api-openapi.yml
  format: yaml
  label: Gcore Streaming API
  slug: gcore-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-streaming-api-openapi.yml
- filename: gcore-waap-api-openapi.yml
  format: yaml
  label: Gcore WAAP API
  slug: gcore-waap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-waap-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gcore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gcore secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gcore
provider_slug: gcore
scheme_count: 1
schemes:
- description: 'Permanent API token sent as "Authorization: APIKey <token>". The header name is case-insensitive.'
  in: header
  name: APIKey
  parameter: Authorization
  sources:
  - openapi/gcore-openapi.yml
  type: apiKey
slug: gcore-authentication
source_filename: gcore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gcore-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Permanent API token sent as \"Authorization: APIKey <token>\". The header name\n    is case-insensitive.'\n  sources:\n  - openapi/gcore-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/authentication/gcore-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Edge Cloud
- CDN
- Streaming
- Edge AI
- Infrastructure
---
