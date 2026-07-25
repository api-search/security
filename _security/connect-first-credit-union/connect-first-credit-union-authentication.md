---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Connect First Credit Union Authentication
name_suffix: Authentication
oauth_flows: []
overview: connectFirst Credit Union declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: connectFirst Credit Union
provider_slug: connect-first-credit-union
scheme_count: 1
schemes:
- endpoints:
    authorization_endpoint: https://www.connectfirstcu.com/umbraco/delivery/api/v1/security/member/authorize
    end_session_endpoint: https://www.connectfirstcu.com/umbraco/delivery/api/v1/security/member/signout
    jwks_uri: https://www.connectfirstcu.com/.well-known/jwks
    revocation_endpoint: https://www.connectfirstcu.com/umbraco/delivery/api/v1/security/member/revoke
    token_endpoint: https://www.connectfirstcu.com/umbraco/delivery/api/v1/security/member/token
  flows:
  - authorization_code
  - refresh_token
  id_token_signing_alg:
  - RS256
  name: oidc_member
  openIdConnectUrl: https://www.connectfirstcu.com/.well-known/openid-configuration
  pkce: true
  pkce_methods:
  - S256
  - plain
  protocol: OpenID Connect / OAuth 2.0
  response_types:
  - code
  scopes_supported:
  - openid
  - offline_access
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: connect-first-credit-union-authentication
source_filename: connect-first-credit-union-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.connectfirstcu.com/.well-known/openid-configuration\nnote: >-\n  Auth profile derived from the live OIDC discovery document. This is Umbraco\n  CMS member authentication for the public connectFirst website, NOT a\n  first-party open-banking or developer data API. There is no public developer\n  portal, no client registration, and the Umbraco Content Delivery API is\n  disabled. Included for completeness of the discovered machine-readable surface.\nissuer: https://www.connectfirstcu.com/\nschemes:\n- name: oidc_member\n  type: openIdConnect\n  protocol: OpenID Connect / OAuth 2.0\n  openIdConnectUrl: https://www.connectfirstcu.com/.well-known/openid-configuration\n  flows:\n  - authorization_code\n  - refresh_token\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  response_types:\n  - code\n  scopes_supported:\n  - openid\n  - offline_access\n  id_token_signing_alg:\n  - RS256\n  token_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  - client_secret_post\n  endpoints:\n    authorization_endpoint: https://www.connectfirstcu.com/umbraco/delivery/api/v1/security/member/authorize\n    token_endpoint: https://www.connectfirstcu.com/umbraco/delivery/api/v1/security/member/token\n    end_session_endpoint: https://www.connectfirstcu.com/umbraco/delivery/api/v1/security/member/signout\n    revocation_endpoint: https://www.connectfirstcu.com/umbraco/delivery/api/v1/security/member/revoke\n    jwks_uri: https://www.connectfirstcu.com/.well-known/jwks\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connect-first-credit-union/refs/heads/main/authentication/connect-first-credit-union-authentication.yml
summary_line: 1 scheme
tags:
- Financial Services
- Banking
- Canada
- Credit Union
- Alberta
- Cooperative
- Data Aggregation
---
