---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ohmconnect Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ohmconnect secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ohmconnect
provider_slug: ohmconnect
scheme_count: 1
schemes:
- authorization_domain: auth-8d7ef420-2340-11ed-8fa1-0e5fb6478cd3.auth.us-east-1.amazoncognito.com
  flows:
  - authorizationUrl: https://auth-8d7ef420-2340-11ed-8fa1-0e5fb6478cd3.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
    - profile
    - openid
    - aws.cognito.signin.user.admin
    tokenUrl: https://auth-8d7ef420-2340-11ed-8fa1-0e5fb6478cd3.auth.us-east-1.amazoncognito.com/oauth2/token
  name: cognito
  provider: AWS Cognito
  region: us-east-1
  sources:
  - https://developer.ohmconnect.com
  type: oauth2
slug: ohmconnect-authentication
source_filename: ohmconnect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.ohmconnect.com (observed OAuth2 redirect to AWS Cognito hosted UI)\nnotes: >-\n  OhmConnect's developer portal (developer.ohmconnect.com) is gated entirely\n  behind AWS Cognito. Unauthenticated requests to any path (including\n  /openapi.json, /docs, /.well-known/*) 307-redirect to the Cognito hosted\n  login/authorize endpoint. The auth profile below is observed from that live\n  redirect; the OpenAPI/spec surface itself is not publicly accessible, so the\n  underlying API security schemes could not be harvested.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\nschemes:\n- name: cognito\n  type: oauth2\n  provider: AWS Cognito\n  authorization_domain: auth-8d7ef420-2340-11ed-8fa1-0e5fb6478cd3.auth.us-east-1.amazoncognito.com\n  region: us-east-1\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://auth-8d7ef420-2340-11ed-8fa1-0e5fb6478cd3.auth.us-east-1.amazoncognito.com/oauth2/authorize\n\
  \    tokenUrl: https://auth-8d7ef420-2340-11ed-8fa1-0e5fb6478cd3.auth.us-east-1.amazoncognito.com/oauth2/token\n    scopes:\n    - profile\n    - openid\n    - aws.cognito.signin.user.admin\n  sources:\n  - https://developer.ohmconnect.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ohmconnect/refs/heads/main/authentication/ohmconnect-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Energy
- Demand Response
- Virtual Power Plant
- Utilities
- Smart Home
- Sustainability
- Electricity
---
