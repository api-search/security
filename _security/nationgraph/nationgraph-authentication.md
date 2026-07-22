---
api_key_in: []
api_specs:
- filename: nationgraph-openapi-original.json
  format: json
  label: NationGraph API
  slug: nationgraph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationgraph/refs/heads/main/openapi/nationgraph-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nationgraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: NationGraph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NationGraph
provider_slug: nationgraph
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/nationgraph-openapi-original.json
  type: http
slug: nationgraph-authentication
source_filename: nationgraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nationgraph-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nationgraph-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationgraph/refs/heads/main/authentication/nationgraph-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Sales Intelligence
- Public Sector
- Government
- SLED
- GovTech
- Procurement
- RFP
- Data
- Sales
---
