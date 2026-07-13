---
api_key_in:
- header
api_specs:
- filename: neighbor-openapi.yml
  format: yaml
  label: Neighbor
  slug: neighbor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neighbor/refs/heads/main/openapi/neighbor-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Neighbor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neighbor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Neighbor
provider_slug: neighbor
scheme_count: 1
schemes:
- description: Use header value `NEIGHBOR-API-KEY <your-api-key>`. Email jon@neighbor.com to request an API key.
  in: header
  name: NeighborApiKey
  parameter: Authorization
  sources:
  - openapi/neighbor-openapi.yml
  type: apiKey
slug: neighbor-authentication
source_filename: neighbor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/neighbor-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: NeighborApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Use header value `NEIGHBOR-API-KEY <your-api-key>`. Email jon@neighbor.com to\n    request an API key.\n  sources:\n  - openapi/neighbor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neighbor/refs/heads/main/authentication/neighbor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Storage
- Marketplace
- Reporting
---
