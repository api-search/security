---
api_key_in: []
api_specs:
- filename: ironclad-clickwrap-activity-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Activity API
  slug: ironclad-clickwrap-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-activity-api-openapi.yml
- filename: ironclad-clickwrap-contracts-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Contracts API
  slug: ironclad-clickwrap-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-contracts-api-openapi.yml
- filename: ironclad-clickwrap-groups-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Groups API
  slug: ironclad-clickwrap-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-groups-api-openapi.yml
- filename: ironclad-clickwrap-signers-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Signers API
  slug: ironclad-clickwrap-signers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-signers-api-openapi.yml
- filename: ironclad-clickwrap-sites-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Sites API
  slug: ironclad-clickwrap-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-sites-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ironclad Clickwrap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ironclad Clickwrap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ironclad Clickwrap
provider_slug: ironclad-clickwrap
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ironclad-clickwrap-openapi.yml
  type: http
slug: ironclad-clickwrap-authentication
source_filename: ironclad-clickwrap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ironclad-clickwrap-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/ironclad-clickwrap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/authentication/ironclad-clickwrap-authentication.yml
summary_line: http · 1 scheme
tags:
- Agreements
- Compliance
- Contracts
- Legal
---
