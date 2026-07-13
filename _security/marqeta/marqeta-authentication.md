---
api_key_in: []
api_specs:
- filename: marqeta-core-api-openapi.yml
  format: yaml
  label: Marqeta Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/openapi/marqeta-core-api-openapi.yml
- filename: marqeta-diva-api-openapi.yml
  format: yaml
  label: Marqeta Diva API
  slug: diva-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/openapi/marqeta-diva-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Marqeta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marqeta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Marqeta
provider_slug: marqeta
scheme_count: 1
schemes:
- name: mqAppAndAccessToken
  scheme: basic
  sources:
  - openapi/marqeta-core-api-openapi.yml
  - openapi/marqeta-diva-api-openapi.yml
  type: http
slug: marqeta-authentication
source_filename: marqeta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marqeta-core-api-openapi.yml, openapi/marqeta-diva-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: mqAppAndAccessToken\n  type: http\n  scheme: basic\n  sources:\n  - openapi/marqeta-core-api-openapi.yml\n  - openapi/marqeta-diva-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/authentication/marqeta-authentication.yml
summary_line: http · 1 scheme
tags:
- FinTech
- BaaS
- Card Issuing
- Payments
- Embedded Finance
---
