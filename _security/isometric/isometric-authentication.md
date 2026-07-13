---
api_key_in: []
api_specs:
- filename: isometric-registry-api-openapi.json
  format: json
  label: Isometric Registry API
  slug: isometric-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isometric/refs/heads/main/openapi/isometric-registry-api-openapi.json
- filename: isometric-certify-api-openapi.json
  format: json
  label: Isometric Certify Data Ingestion API
  slug: isometric-certify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isometric/refs/heads/main/openapi/isometric-certify-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Isometric Authentication
name_suffix: Authentication
oauth_flows: []
overview: Isometric secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Isometric
provider_slug: isometric
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'A JWT Bearer token header for authentication and authorization, in the format `Authorization: Bearer <token>`'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/isometric-certify-api-openapi.json
  - openapi/isometric-registry-api-openapi.json
  type: http
slug: isometric-authentication
source_filename: isometric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/isometric-certify-api-openapi.json, openapi/isometric-registry-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'A JWT Bearer token header for authentication and authorization, in the format\n    `Authorization: Bearer <token>`'\n  sources:\n  - openapi/isometric-certify-api-openapi.json\n  - openapi/isometric-registry-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isometric/refs/heads/main/authentication/isometric-authentication.yml
summary_line: http · 1 scheme
tags:
- Carbon Removal
- Carbon Registry
- Climate
- Climate Tech
- CDR
- MRV
- Measurement Reporting Verification
- Certification
- Superpollutants
- Biochar
- Direct Air Capture
- Enhanced Weathering
- Mineralization
- Reforestation
- Mangrove Restoration
- Agroforestry
- Methane
- HFC
- Sustainability
- ESG
- Net Zero
- LCA
- Greenhouse Gas
- Protocols
- AI
- MCP
---
