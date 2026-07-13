---
api_key_in: []
api_specs:
- filename: thumbtack-demand-openapi.yml
  format: yaml
  label: Thumbtack Demand API
  slug: thumbtack-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-demand-openapi.yml
- filename: thumbtack-pro-openapi.yml
  format: yaml
  label: Thumbtack Pro API
  slug: thumbtack-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-pro-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Thumbtack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Thumbtack secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Thumbtack
provider_slug: thumbtack
scheme_count: 3
schemes:
- description: Used by legacy v1/v2 routes.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/thumbtack-demand-openapi.yml
  - openapi/thumbtack-pro-openapi.yml
  type: http
- description: Used by v4 routes. Authorization Code and Client Credentials flows.
  flows:
  - authorizationUrl: https://www.thumbtack.com/services/partner-connect/
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.thumbtack.com/v4/oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.thumbtack.com/v4/oauth/token
  name: oauth2
  sources:
  - openapi/thumbtack-demand-openapi.yml
  type: oauth2
- description: Bearer token obtained via the partner-connect authorization code flow.
  flows:
  - authorizationUrl: https://www.thumbtack.com/services/partner-connect/
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://pro-api.thumbtack.com/v2/tokens/access
  name: oauth2
  sources:
  - openapi/thumbtack-pro-openapi.yml
  type: oauth2
slug: thumbtack-authentication
source_filename: thumbtack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thumbtack-demand-openapi.yml, openapi/thumbtack-pro-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Used by legacy v1/v2 routes.\n  sources:\n  - openapi/thumbtack-demand-openapi.yml\n  - openapi/thumbtack-pro-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.thumbtack.com/services/partner-connect/\n    tokenUrl: https://api.thumbtack.com/v4/oauth/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://api.thumbtack.com/v4/oauth/token\n    scopes: 0\n  description: Used by v4 routes. Authorization Code and Client Credentials flows.\n  sources:\n  - openapi/thumbtack-demand-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.thumbtack.com/services/partner-connect/\n\
  \    tokenUrl: https://pro-api.thumbtack.com/v2/tokens/access\n    scopes: 0\n  description: Bearer token obtained via the partner-connect authorization code flow.\n  sources:\n  - openapi/thumbtack-pro-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/authentication/thumbtack-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Local Services
- Marketplace
- Home Services
- Leads
- Partner API
---
