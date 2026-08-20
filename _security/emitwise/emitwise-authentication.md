---
api_key_in: []
api_specs:
- filename: emitwise-facilities-api-openapi.yml
  format: yaml
  label: Emitwise Facilities API
  slug: emitwise-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-facilities-api-openapi.yml
- filename: emitwise-files-api-openapi.yml
  format: yaml
  label: Emitwise Files API
  slug: emitwise-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-files-api-openapi.yml
- filename: emitwise-projects-api-openapi.yml
  format: yaml
  label: Emitwise Projects API
  slug: emitwise-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-projects-api-openapi.yml
- filename: emitwise-schema-api-openapi.yml
  format: yaml
  label: Emitwise Schema API
  slug: emitwise-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-schema-api-openapi.yml
- filename: emitwise-suppliers-api-openapi.yml
  format: yaml
  label: Emitwise Suppliers API
  slug: emitwise-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-suppliers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Emitwise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emitwise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Emitwise
provider_slug: emitwise
scheme_count: 1
schemes:
- description: Emitwise API key generated from Company settings, presented as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/emitwise-api-openapi.yml
  type: http
slug: emitwise-authentication
source_filename: emitwise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/emitwise-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Emitwise API key generated from Company settings, presented as a Bearer token.\n  sources:\n  - openapi/emitwise-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/authentication/emitwise-authentication.yml
summary_line: http · 1 scheme
tags:
- Carbon Accounting
- Greenhouse Gas
- Scope 3
- Supply Chain Emissions
- Product Carbon Footprint
- Sustainability
- ESG
- CDP
- CSRD
- GHG Protocol
- Climate
- Procurement
- Artificial Intelligence
---
