---
api_key_in: []
api_specs:
- filename: streamone-ion-openapi.yml
  format: yaml
  label: TD SYNNEX StreamOne Ion API
  slug: streamone-ion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/streamone-ion-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tech Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tech Data secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tech Data
provider_slug: tech-data
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer token obtained via the /oauth/token endpoint.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/streamone-ion-openapi.yml
  type: http
slug: tech-data-authentication
source_filename: tech-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/streamone-ion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token obtained via the /oauth/token endpoint.\n  sources:\n  - openapi/streamone-ion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/authentication/tech-data-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Distribution
- Information Technology
- Partner
- Fortune 500
---
