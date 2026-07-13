---
api_key_in: []
api_specs:
- filename: bynder-openapi.yml
  format: yaml
  label: Bynder API
  slug: bynder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bynder Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Bynder secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Bynder
provider_slug: bynder
scheme_count: 1
schemes:
- description: OAuth 2.0 with JWT bearer access tokens
  flows:
  - authorizationUrl: https://yourportal.bynder.com/v6/authentication/oauth2/auth
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials
  name: oauth2
  sources:
  - openapi/bynder-openapi.yml
  type: oauth2
slug: bynder-authentication
source_filename: bynder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bynder-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://yourportal.bynder.com/v6/authentication/oauth2/auth\n    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization\n    scopes: 7\n  - flow: clientCredentials\n    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials\n    scopes: 2\n  description: OAuth 2.0 with JWT bearer access tokens\n  sources:\n  - openapi/bynder-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/authentication/bynder-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Digital Asset Management
- DAM
- Brand Management
- Content Management
- Marketing
---
