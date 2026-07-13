---
api_key_in: []
api_specs:
- filename: microcks-openapi.yml
  format: yaml
  label: Microcks API
  slug: microcks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microcks/refs/heads/main/openapi/microcks-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microcks Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Microcks secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Microcks
provider_slug: microcks
scheme_count: 1
schemes:
- description: JWT Bearer acquired using OAuth 2 Authentication flow or Direct Access Grant
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://keycloak.example.com/realms/microcks/protocol/openid-connect/token
  name: jwt-bearer
  sources:
  - openapi/microcks-openapi.yml
  type: oauth2
slug: microcks-authentication
source_filename: microcks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microcks-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: jwt-bearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://keycloak.example.com/realms/microcks/protocol/openid-connect/token\n    scopes: 3\n  description: JWT Bearer acquired using OAuth 2 Authentication flow or Direct Access Grant\n  sources:\n  - openapi/microcks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microcks/refs/heads/main/authentication/microcks-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- API Testing
- Cloud Native
- DevOps
- Mocking
- Open Source
---
