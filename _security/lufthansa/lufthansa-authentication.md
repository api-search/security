---
api_key_in: []
api_specs:
- filename: lufthansa-openapi.yml
  format: yaml
  label: Lufthansa Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lufthansa/refs/heads/main/openapi/lufthansa-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lufthansa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lufthansa secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lufthansa
provider_slug: lufthansa
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.lufthansa.com/v1/oauth/token
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.lufthansa.com/v1/oauth/token
  name: auth
  sources:
  - openapi/lufthansa-openapi.yml
  type: oauth2
slug: lufthansa-authentication
source_filename: lufthansa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lufthansa-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.lufthansa.com/v1/oauth/token\n    tokenUrl: https://api.lufthansa.com/v1/oauth/token\n    scopes: 1\n  sources:\n  - openapi/lufthansa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lufthansa/refs/heads/main/authentication/lufthansa-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Airlines
- Travel
- Aviation
- Flights
---
