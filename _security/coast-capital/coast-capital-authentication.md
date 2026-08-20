---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Coast Capital Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Coast Capital Savings secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Coast Capital Savings
provider_slug: coast-capital
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - plain
  - S256
  endpoints:
    authorization: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/authorize
    end_session: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/signout
    jwks: https://www.coastcapitalsavings.com/.well-known/jwks
    revocation: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/revoke
    token: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/token
    userinfo: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/userinfo
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://www.coastcapitalsavings.com/
  name: memberOIDC
  openIdConnectUrl: https://www.coastcapitalsavings.com/.well-known/openid-configuration
  require_pushed_authorization_requests: false
  response_modes_supported:
  - query
  - form_post
  - fragment
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - offline_access
  sources:
  - well-known/coast-capital-openid-configuration.json
  tls_client_certificate_bound_access_tokens: false
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  type: openIdConnect
slug: coast-capital-authentication
source_filename: coast-capital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.coastcapitalsavings.com/.well-known/openid-configuration\nnote: >-\n  Derived from the live member-authentication OIDC discovery document. This is\n  the identity-provider surface used for member sign-in (Umbraco member-auth\n  delivery API), NOT authentication for a public banking/data API — Coast Capital\n  publishes no public first-party API. Recorded here because it is a real,\n  anonymously-fetchable auth surface.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  pkce: [S256, plain]\n  audience: member-authentication\nschemes:\n- name: memberOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.coastcapitalsavings.com/.well-known/openid-configuration\n  issuer: https://www.coastcapitalsavings.com/\n  sources: [well-known/coast-capital-openid-configuration.json]\n  endpoints:\n    authorization: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/authorize\n\
  \    token: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/token\n    userinfo: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/userinfo\n    revocation: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/revoke\n    end_session: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/signout\n    jwks: https://www.coastcapitalsavings.com/.well-known/jwks\n  grant_types_supported: [authorization_code, refresh_token, client_credentials]\n  response_types_supported: [code]\n  response_modes_supported: [query, form_post, fragment]\n  scopes_supported: [openid, offline_access]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [plain, S256]\n  token_endpoint_auth_methods_supported: [client_secret_post, private_key_jwt, client_secret_basic]\n  require_pushed_authorization_requests: false\n  tls_client_certificate_bound_access_tokens: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coast-capital/refs/heads/main/authentication/coast-capital-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative
- Consumer-Driven Banking
- Data Aggregation
---
