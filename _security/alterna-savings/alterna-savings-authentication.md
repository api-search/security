---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Alterna Savings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alterna Savings declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Alterna Savings
provider_slug: alterna-savings
scheme_count: 1
schemes:
- endpoints:
    authorization: https://www.alterna.ca/umbraco/delivery/api/v1/security/member/authorize
    end_session: https://www.alterna.ca/umbraco/delivery/api/v1/security/member/signout
    jwks: https://www.alterna.ca/.well-known/jwks
    revocation: https://www.alterna.ca/umbraco/delivery/api/v1/security/member/revoke
    token: https://www.alterna.ca/umbraco/delivery/api/v1/security/member/token
  flows:
  - authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: umbraco_member_oidc
  id_token_signing_alg:
  - RS256
  issuer: https://www.alterna.ca/
  pkce:
    code_challenge_methods:
    - plain
    - S256
    supported: true
  protocol: OpenID Connect / OAuth 2.0
  response_types_supported:
  - code
  scopes:
  - openid
  - offline_access
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: alterna-savings-authentication
source_filename: alterna-savings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.alterna.ca/.well-known/openid-configuration\nnote: >-\n  Derived from the live OpenID Connect / OAuth2 authorization-server metadata the\n  site publishes. This is the Umbraco CMS \"Delivery API\" MEMBER-authentication\n  surface behind the website's member login — NOT a banking or developer API.\n  Alterna publishes no first-party developer API or its own auth documentation;\n  this profile records only the anonymously discoverable protocol metadata.\nschemes:\n- id: umbraco_member_oidc\n  type: oauth2\n  protocol: OpenID Connect / OAuth 2.0\n  flows:\n  - authorization_code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - plain\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - offline_access\n\
  \  issuer: https://www.alterna.ca/\n  endpoints:\n    authorization: https://www.alterna.ca/umbraco/delivery/api/v1/security/member/authorize\n    token: https://www.alterna.ca/umbraco/delivery/api/v1/security/member/token\n    end_session: https://www.alterna.ca/umbraco/delivery/api/v1/security/member/signout\n    revocation: https://www.alterna.ca/umbraco/delivery/api/v1/security/member/revoke\n    jwks: https://www.alterna.ca/.well-known/jwks\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alterna-savings/refs/heads/main/authentication/alterna-savings-authentication.yml
summary_line: 1 scheme
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative
- Consumer-Driven Banking
- Interac
- Data Aggregation
---
