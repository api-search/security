---
api_key_in: []
api_specs:
- filename: taboola-backstage-campaigns-api-openapi.yml
  format: yaml
  label: Taboola Backstage Campaigns API
  slug: taboola-backstage-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-campaigns-api-openapi.yml
- filename: taboola-backstage-items-api-openapi.yml
  format: yaml
  label: Taboola Backstage Campaign Items API
  slug: taboola-backstage-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-items-api-openapi.yml
- filename: taboola-backstage-audiences-api-openapi.yml
  format: yaml
  label: Taboola Backstage Audiences API
  slug: taboola-backstage-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-audiences-api-openapi.yml
- filename: taboola-backstage-conversions-api-openapi.yml
  format: yaml
  label: Taboola Backstage Conversions API
  slug: taboola-backstage-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-conversions-api-openapi.yml
- filename: taboola-backstage-reports-api-openapi.yml
  format: yaml
  label: Taboola Backstage Reports API
  slug: taboola-backstage-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-reports-api-openapi.yml
- filename: taboola-backstage-dictionary-api-openapi.yml
  format: yaml
  label: Taboola Backstage Dictionary API
  slug: taboola-backstage-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-dictionary-api-openapi.yml
- filename: taboola-backstage-accounts-api-openapi.yml
  format: yaml
  label: Taboola Backstage Accounts API
  slug: taboola-backstage-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-accounts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Taboola Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taboola secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Taboola
provider_slug: taboola
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/taboola-backstage-accounts-api-openapi.yml
  - openapi/taboola-backstage-audiences-api-openapi.yml
  - openapi/taboola-backstage-campaigns-api-openapi.yml
  - openapi/taboola-backstage-conversions-api-openapi.yml
  - openapi/taboola-backstage-dictionary-api-openapi.yml
  - openapi/taboola-backstage-items-api-openapi.yml
  - openapi/taboola-backstage-reports-api-openapi.yml
  type: http
slug: taboola-authentication
source_filename: taboola-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taboola-backstage-accounts-api-openapi.yml, openapi/taboola-backstage-audiences-api-openapi.yml,\n  openapi/taboola-backstage-campaigns-api-openapi.yml, openapi/taboola-backstage-conversions-api-openapi.yml,\n  openapi/taboola-backstage-dictionary-api-openapi.yml, openapi/taboola-backstage-items-api-openapi.yml,\n  openapi/taboola-backstage-reports-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/taboola-backstage-accounts-api-openapi.yml\n  - openapi/taboola-backstage-audiences-api-openapi.yml\n  - openapi/taboola-backstage-campaigns-api-openapi.yml\n  - openapi/taboola-backstage-conversions-api-openapi.yml\n  - openapi/taboola-backstage-dictionary-api-openapi.yml\n  - openapi/taboola-backstage-items-api-openapi.yml\n  - openapi/taboola-backstage-reports-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/authentication/taboola-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- Native Advertising
- Discovery
- Performance Marketing
- AdTech
- Realize
- Backstage
- Recommendation
- Publisher
- Programmatic
---
