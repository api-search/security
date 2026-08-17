---
api_key_in: []
api_specs:
- filename: osmaura-prospect-openapi.yml
  format: yaml
  label: Osmaura Prospect API
  slug: osmaura-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmaura/refs/heads/main/openapi/osmaura-prospect-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Osmaura Authentication
name_suffix: Authentication
oauth_flows: []
overview: Osmaura secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Osmaura
provider_slug: osmaura
scheme_count: 1
schemes:
- bearerFormat: API key
  description: Tenant-scoped production read key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/osmaura-prospect-openapi.yml
  type: http
slug: osmaura-authentication
source_filename: osmaura-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/osmaura-prospect-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: Tenant-scoped production read key.\n  sources:\n  - openapi/osmaura-prospect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmaura/refs/heads/main/authentication/osmaura-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Legal
- LegalTech
- Artificial Intelligence
- Sales Enablement
- Business Development
- Y Combinator
- Market Intelligence
- Data
- Government Data
- Prospecting
---
