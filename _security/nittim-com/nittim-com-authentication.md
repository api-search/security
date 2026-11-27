---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nittim-com-audit-api-openapi.yml
  format: yaml
  label: Nittim Audit API
  slug: nittim-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nittim-com/openapi/nittim-com-audit-api-openapi.yml
- filename: nittim-com-reports-api-openapi.yml
  format: yaml
  label: Nittim Reports API
  slug: nittim-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nittim-com/openapi/nittim-com-reports-api-openapi.yml
- filename: nittim-com-source-api-openapi.yml
  format: yaml
  label: Nittim Source API
  slug: nittim-com-source-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nittim-com/openapi/nittim-com-source-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nittim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nittim secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nittim
provider_slug: nittim-com
scheme_count: 1
schemes:
- bearerFormat: nittim_sk_…
  description: 'A nittim API key (Authorization: Bearer nittim_sk_…). Mint one at https://nittim.com/keys.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nittim-com-openapi.json
  type: http
slug: nittim-com-authentication
source_filename: nittim-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nittim-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: nittim_sk_…\n  description: 'A nittim API key (Authorization: Bearer nittim_sk_…). Mint one at https://nittim.com/keys.'\n  sources:\n  - openapi/nittim-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nittim-com/authentication/nittim-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- AI Assistant
---
