---
api_key_in:
- header
api_specs:
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore CDN API
  slug: cdn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Cloud API
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Object Storage API
  slug: storage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore DNS API
  slug: dns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Streaming API
  slug: streaming
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Everywhere Inference API
  slug: inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Security & WAAP API
  slug: security-waap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore FastEdge API
  slug: fastedge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
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
