---
api_key_in: []
api_specs:
- filename: alphaloops-carriers-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Carriers API
  slug: alphaloops-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-carriers-api-openapi.yml
- filename: alphaloops-contacts-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Contacts API
  slug: alphaloops-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-contacts-api-openapi.yml
- filename: alphaloops-inspections-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Inspections API
  slug: alphaloops-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-inspections-api-openapi.yml
- filename: alphaloops-vins-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Vins API
  slug: alphaloops-vins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-vins-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alphaloops Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlphaLoops FMCSA Carrier Data API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AlphaLoops FMCSA Carrier Data API
provider_slug: alphaloops
scheme_count: 1
schemes:
- description: 'API key provided by AlphaLoops. Include as: Authorization: Bearer YOUR_API_KEY'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alphaloops-fmcsa-carrier-data-api-openapi.json
  type: http
slug: alphaloops-authentication
source_filename: alphaloops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: derived\nsource: openapi/alphaloops-fmcsa-carrier-data-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key provided by AlphaLoops. Include as: Authorization: Bearer YOUR_API_KEY'\n  sources:\n  - openapi/alphaloops-fmcsa-carrier-data-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/authentication/alphaloops-authentication.yml
summary_line: http · 1 scheme
tags:
- fmcsa api
- safer web api
- dot lookup
- carrier data
- freight
- trucking
- motor carrier
- fleet intelligence
- Sales Intelligence
- mcp server
- contact enrichment
- risk
- fraud
---
