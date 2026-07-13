---
api_key_in: []
api_specs:
- filename: granular-farm-management-openapi.yml
  format: yaml
  label: Granular Farm Management API
  slug: granular-farm-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/granular/refs/heads/main/openapi/granular-farm-management-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Granular Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Granular (Corteva Agriscience) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Granular (Corteva Agriscience)
provider_slug: granular
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://auth.granular.ag/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://auth.granular.ag/oauth/token
  name: OAuth2
  sources:
  - openapi/granular-farm-management-openapi.yml
  type: oauth2
slug: granular-authentication
source_filename: granular-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/granular-farm-management-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.granular.ag/oauth/authorize\n    tokenUrl: https://auth.granular.ag/oauth/token\n    scopes: 2\n  sources:\n  - openapi/granular-farm-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granular/refs/heads/main/authentication/granular-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Agriculture
- Farm Management
- Financial
- Crop Planning
- Agronomy
---
