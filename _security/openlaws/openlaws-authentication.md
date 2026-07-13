---
api_key_in: []
api_specs:
- filename: openlaws-openapi.yml
  format: yaml
  label: OpenLaws Legal Data API
  slug: openlaws
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/openapi/openlaws-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openlaws Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenLaws secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenLaws
provider_slug: openlaws
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Authenticate API requests via a bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openlaws-openapi.json
  - openapi/openlaws-openapi.yml
  type: http
slug: openlaws-authentication
source_filename: openlaws-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openlaws-openapi.json, openapi/openlaws-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Authenticate API requests via a bearer token\n  sources:\n  - openapi/openlaws-openapi.json\n  - openapi/openlaws-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/authentication/openlaws-authentication.yml
summary_line: http · 1 scheme
tags:
- Legal
- Law
- Statutes
- Regulations
- Constitutions
- Case Law
- Citations
- Search
- RAG
- LegalTech
- RegTech
- Compliance
- GRC
- Government Data
---
