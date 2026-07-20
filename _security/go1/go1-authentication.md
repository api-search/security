---
api_key_in: []
api_specs:
- filename: go1-openapi.yml
  format: yaml
  label: Go1 API
  slug: go1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Go1 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Go1 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Go1
provider_slug: go1
scheme_count: 1
schemes:
- description: OAuth 2.0. Server-to-server integrations use the client_credentials flow; user-context integrations use the authorization_code flow. Access tokens are valid for 12 hours.
  flows:
  - flow: clientCredentials
    scopes: 8
    tokenUrl: https://auth.go1.com/oauth/token
  - authorizationUrl: https://auth.go1.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://auth.go1.com/oauth/token
  name: OAuth2
  sources:
  - openapi/go1-openapi.yml
  type: oauth2
slug: go1-authentication
source_filename: go1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/go1-openapi.yml\ndocs: https://developers.go1.com/docs/developer-tools/auth/overview-auth\nverified:\n- https://developers.go1.com/docs/developer-tools/auth/grant-client-credentials\n- POST https://auth.go1.com/oauth/token returned 400 invalid_request (live probe, endpoint confirmed)\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.go1.com/oauth/token\n    scopes: 8\n  - flow: authorizationCode\n    authorizationUrl: https://auth.go1.com/oauth/authorize\n    tokenUrl: https://auth.go1.com/oauth/token\n    scopes: 8\n  description: OAuth 2.0. Server-to-server integrations use the client_credentials flow; user-context\n    integrations use the authorization_code flow. Access tokens are valid for 12 hours.\n  sources:\n  - openapi/go1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/authentication/go1-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Edtech
- Learning
- E-Learning
- Corporate Training
- Content
- Learning Management
- LMS
- Education
- Webhooks
---
