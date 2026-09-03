---
api_key_in: []
api_specs:
- filename: api-dash-openapi.yml
  format: yaml
  label: API Dash
  slug: api-dash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-openapi.yml
- filename: api-dash-openapi.yml
  format: yaml
  label: API Dash APIs
  slug: api-dash-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Api Dash Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: API Dash secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: API Dash
provider_slug: api-dash
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: /login
  name: OAuth2PasswordBearer
  sources:
  - openapi/api-dash-openapi.yml
  type: oauth2
slug: api-dash-authentication
source_filename: api-dash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/api-dash-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /login\n    scopes: 0\n  sources:\n  - openapi/api-dash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/authentication/api-dash-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- API Client
- Open-Source
- Flutter
- Desktop
- Mobile
---
