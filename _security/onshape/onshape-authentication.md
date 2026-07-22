---
api_key_in: []
api_specs:
- filename: onshape-openapi-original.json
  format: json
  label: Onshape REST API
  slug: onshape-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onshape/refs/heads/main/openapi/onshape-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Onshape Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Onshape secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Onshape
provider_slug: onshape
scheme_count: 2
schemes:
- description: Use OAuth 2.0 to authenticate requests.
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 24
    tokenUrl: /oauth/token
  name: OAuth2
  sources:
  - openapi/onshape-openapi-original.json
  type: oauth2
- description: Use Basic Authentication with API Keys (key as username and secret as password) to authenticate requests.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/onshape-openapi-original.json
  type: http
slug: onshape-authentication
source_filename: onshape-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/onshape-openapi-original.json\ndocs: https://onshape-public.github.io/docs/auth/\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 24\n  description: Use OAuth 2.0 to authenticate requests.\n  sources:\n  - openapi/onshape-openapi-original.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Use Basic Authentication with API Keys (key as username and secret as password)\n    to authenticate requests.\n  sources:\n  - openapi/onshape-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onshape/refs/heads/main/authentication/onshape-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- CAD
- PLM
- Product Data Management
- Engineering
- Manufacturing
- Design
- Cloud
- Developer Tools
---
