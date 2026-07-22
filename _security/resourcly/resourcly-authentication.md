---
api_key_in:
- header
api_specs:
- filename: resourcly-openapi-original.json
  format: json
  label: Resourcly API
  slug: resourcly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resourcly/refs/heads/main/openapi/resourcly-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Resourcly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Resourcly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Resourcly
provider_slug: resourcly
scheme_count: 1
schemes:
- description: 'Firebase JWT token. Format: "Bearer {token}"'
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/resourcly-openapi-original.json
  type: apiKey
slug: resourcly-authentication
source_filename: resourcly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/resourcly-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Firebase JWT token. Format: \"Bearer {token}\"'\n  sources:\n  - openapi/resourcly-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resourcly/refs/heads/main/authentication/resourcly-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Manufacturing
- Inventory Optimization
- PLM
- ERP
- Procurement
- Supply Chain
- Artificial Intelligence
- Data Harmonization
- Similarity Search
- BOM
---
