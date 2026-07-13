---
api_key_in: []
api_specs:
- filename: high-mobility-openapi.yml
  format: yaml
  label: High Mobility Vehicle API
  slug: high-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/high-mobility/refs/heads/main/openapi/high-mobility-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: High Mobility Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: High Mobility secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: High Mobility
provider_slug: high-mobility
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.high-mobility.com/v1/access_token
  - authorizationUrl: https://owner-panel.high-mobility.com/oauth/new
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.high-mobility.com/v1/access_token
  name: oauth2
  sources:
  - openapi/high-mobility-openapi.yml
  type: oauth2
slug: high-mobility-authentication
source_filename: high-mobility-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/high-mobility-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.high-mobility.com/v1/access_token\n    scopes: 1\n  - flow: authorizationCode\n    authorizationUrl: https://owner-panel.high-mobility.com/oauth/new\n    tokenUrl: https://api.high-mobility.com/v1/access_token\n    scopes: 1\n  sources:\n  - openapi/high-mobility-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/high-mobility/refs/heads/main/authentication/high-mobility-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automotive
- Connected Cars
- IoT
- Vehicle Data
---
