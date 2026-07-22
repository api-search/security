---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Mudflap Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Mudflap secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Mudflap
provider_slug: mudflap
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://api.mudflapinc.com/oauth/authorize
    flow: authorizationCode
    scopes:
    - openid
    - profile
    - email
    tokenUrl: https://api.mudflapinc.com/oauth/token
  - flow: password
    scopes:
    - openid
    - profile
    - email
    tokenUrl: https://api.mudflapinc.com/oauth/token
  name: OAuth2
  response_types_supported:
  - code
  revocation_endpoint: https://api.mudflapinc.com/oauth_logout
  source: https://api.mudflapinc.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- claims_supported:
  - sub
  - email
  - name
  - preferred_username
  id_token_signing_alg_values_supported:
  - RS256
  name: OpenIDConnect
  source: https://api.mudflapinc.com/.well-known/oauth-authorization-server
  subject_types_supported:
  - public
  type: openIdConnect
slug: mudflap-authentication
source_filename: mudflap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.mudflapinc.com/.well-known/oauth-authorization-server\ndocs: https://api.mudflapinc.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - password\n  oidc: true\nissuer: https://dashboard.mudflapinc.com\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://api.mudflapinc.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.mudflapinc.com/oauth/authorize\n    tokenUrl: https://api.mudflapinc.com/oauth/token\n    scopes:\n    - openid\n    - profile\n    - email\n  - flow: password\n    tokenUrl: https://api.mudflapinc.com/oauth/token\n    scopes:\n    - openid\n    - profile\n    - email\n  revocation_endpoint: https://api.mudflapinc.com/oauth_logout\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n\
  - name: OpenIDConnect\n  type: openIdConnect\n  source: https://api.mudflapinc.com/.well-known/oauth-authorization-server\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - sub\n  - email\n  - name\n  - preferred_username\nnotes: >-\n  Derived from the RFC 8414 OAuth 2.0 Authorization Server Metadata document\n  published at api.mudflapinc.com. Mudflap runs an OAuth2 / OIDC provider\n  (authorization_code + resource-owner password grants, RS256 id_tokens).\n  No public OpenAPI is published; the protected API surface behind this\n  authorization server is partner/fleet-facing and not publicly documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mudflap/refs/heads/main/authentication/mudflap-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Fintech
- Fuel
- Trucking
- Payments
- Fleet Management
- Logistics
- Fuel Card
---
