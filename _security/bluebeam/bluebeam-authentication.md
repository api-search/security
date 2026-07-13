---
api_key_in: []
api_specs:
- filename: bluebeam-studio-openapi.yml
  format: yaml
  label: Bluebeam Studio API
  slug: bluebeam-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluebeam/refs/heads/main/openapi/bluebeam-studio-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bluebeam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: bluebeam secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: bluebeam
provider_slug: bluebeam
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://authserver.bluebeam.com/auth/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://authserver.bluebeam.com/auth/oauth/token
  name: oauth2
  sources:
  - openapi/bluebeam-studio-openapi.yml
  type: oauth2
slug: bluebeam-authentication
source_filename: bluebeam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bluebeam-studio-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.bluebeam.com/auth/oauth/authorize\n    tokenUrl: https://authserver.bluebeam.com/auth/oauth/token\n    scopes: 3\n  sources:\n  - openapi/bluebeam-studio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluebeam/refs/heads/main/authentication/bluebeam-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
