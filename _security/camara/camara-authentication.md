---
api_key_in: []
api_specs:
- filename: camara-openapi.yml
  format: yaml
  label: CAMARA Quality On Demand API
  slug: quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara/refs/heads/main/openapi/camara-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Camara Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CAMARA secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CAMARA
provider_slug: camara
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.example.com/oauth2/token
  name: oAuth2ClientCredentials
  sources:
  - openapi/camara-openapi.yml
  type: oauth2
slug: camara-authentication
source_filename: camara-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/camara-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.example.com/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/camara-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camara/refs/heads/main/authentication/camara-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Telecom
- Network APIs
- Standards
- Linux Foundation
- Open Gateway
- GSMA
- Connectivity
- 5G
---
