---
api_key_in: []
api_specs:
- filename: productiv-developer-openapi.yml
  format: yaml
  label: Productiv Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-developer-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Productiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Productiv secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Productiv
provider_slug: productiv
scheme_count: 1
schemes:
- bearerFormat: OAuth2
  description: Bearer token obtained from the OAuth2 token endpoint at https://login.api.productiv.com/oauth2/token using client credentials grant type.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/productiv-developer-openapi.yml
  type: http
slug: productiv-authentication
source_filename: productiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/productiv-developer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  description: Bearer token obtained from the OAuth2 token endpoint at https://login.api.productiv.com/oauth2/token\n    using client credentials grant type.\n  sources:\n  - openapi/productiv-developer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/authentication/productiv-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
---
