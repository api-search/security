---
api_key_in: []
api_specs:
- filename: cnh-fieldops-openapi.yml
  format: yaml
  label: CNH FieldOps API
  slug: cnh-fieldops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-fieldops-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cnh Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CNH secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CNH
provider_slug: cnh
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://develop.cnh.com/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://develop.cnh.com/oauth/token
  name: oauth2
  sources:
  - openapi/cnh-fieldops-openapi.yml
  type: oauth2
slug: cnh-authentication
source_filename: cnh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cnh-fieldops-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://develop.cnh.com/oauth/authorize\n    tokenUrl: https://develop.cnh.com/oauth/token\n    scopes: 5\n  sources:\n  - openapi/cnh-fieldops-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/authentication/cnh-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Agriculture
- Construction
- Telematics
- Equipment
- FieldOps
---
