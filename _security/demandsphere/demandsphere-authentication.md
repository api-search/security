---
api_key_in:
- query
api_specs:
- filename: demandsphere-openapi-original.json
  format: json
  label: DemandSphere API v5.0
  slug: demandsphere-api-v50
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandsphere/refs/heads/main/openapi/demandsphere-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Demandsphere Authentication
name_suffix: Authentication
oauth_flows: []
overview: DemandSphere secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DemandSphere
provider_slug: demandsphere
scheme_count: 1
schemes:
- in: query
  name: ApiKey
  parameter: api_key
  sources:
  - openapi/demandsphere-openapi-original.json
  type: apiKey
slug: demandsphere-authentication
source_filename: demandsphere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/demandsphere-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/demandsphere-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandsphere/refs/heads/main/authentication/demandsphere-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- SEO
- Search Intelligence
- SERP Analytics
- AI Search
- LLM Visibility
- Rank Tracking
- Analytics
- API
- MCP
---
