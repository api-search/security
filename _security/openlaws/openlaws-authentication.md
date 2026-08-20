---
api_key_in: []
api_specs:
- filename: openlaws-courts-api-openapi.yml
  format: yaml
  label: OpenLaws Courts API
  slug: openlaws-courts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/openapi/openlaws-courts-api-openapi.yml
- filename: openlaws-jurisdictions-api-openapi.yml
  format: yaml
  label: OpenLaws Jurisdictions API
  slug: openlaws-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/openapi/openlaws-jurisdictions-api-openapi.yml
- filename: openlaws-law-divisions-api-openapi.yml
  format: yaml
  label: OpenLaws Law Divisions API
  slug: openlaws-law-divisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/openapi/openlaws-law-divisions-api-openapi.yml
- filename: openlaws-laws-api-openapi.yml
  format: yaml
  label: OpenLaws Laws API
  slug: openlaws-laws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/openapi/openlaws-laws-api-openapi.yml
- filename: openlaws-opinions-api-openapi.yml
  format: yaml
  label: OpenLaws Opinions API
  slug: openlaws-opinions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/openapi/openlaws-opinions-api-openapi.yml
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
- Legal Tech
- RegTech
- Compliance
- GRC
- Government Data
---
