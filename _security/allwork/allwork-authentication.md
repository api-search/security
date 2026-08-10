---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Allwork Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- password
- refreshToken
- deviceCode
- ciba
- tokenExchange
overview: AllWork secures its APIs with openIdConnect, oauth2, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, password, refreshToken, deviceCode, ciba, and tokenExchange flow(s).
provider_name: AllWork
provider_slug: allwork
scheme_count: 3
schemes:
- issuer: https://auth.allworknow.com/realms/AWN1
  name: allworkOIDC
  openIdConnectUrl: https://auth.allworknow.com/realms/AWN1/.well-known/openid-configuration
  sources:
  - well-known/allwork-openid-configuration.json
  type: openIdConnect
- acr_values_supported:
  - '0'
  - '1'
  claims_supported:
  - aud
  - sub
  - iss
  - auth_time
  - name
  - given_name
  - family_name
  - preferred_username
  - email
  - acr
  code_challenge_methods_supported:
  - plain
  - S256
  endpoints:
    authorization: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth
    backchannel_authentication: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/ext/ciba/auth
    device_authorization: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth/device
    dynamic_client_registration: https://auth.allworknow.com/realms/AWN1/clients-registrations/openid-connect
    end_session: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/logout
    introspection: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token/introspect
    jwks: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/certs
    pushed_authorization_request: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/ext/par/request
    revocation: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/revoke
    token: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token
    userinfo: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/userinfo
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg_values_supported:
  - PS384
  - ES384
  - RS384
  - HS256
  - HS512
  - ES256
  - RS256
  - HS384
  - ES512
  - PS256
  - PS512
  - RS512
  name: allworkOAuth2
  request_parameter_supported: true
  require_pushed_authorization_requests: false
  response_modes_supported:
  - query
  - fragment
  - form_post
  - query.jwt
  - fragment.jwt
  - form_post.jwt
  - jwt
  response_types_supported:
  - code
  - none
  - id_token
  - token
  - id_token token
  - code id_token
  - code token
  - code id_token token
  sources:
  - well-known/allwork-openid-configuration.json
  subject_types_supported:
  - public
  - pairwise
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: oauth2
- name: allworkMutualTLS
  note: tls_client_certificate_bound_access_tokens is true and mtls_endpoint_aliases are advertised; tls_client_auth is an accepted client authentication method.
  sources:
  - well-known/allwork-openid-configuration.json
  type: mutualTLS
slug: allwork-authentication
source_filename: allwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://auth.allworknow.com/realms/AWN1/.well-known/openid-configuration\nnote: >-\n  Derived from AllWork's own live OpenID Connect discovery document, not from an\n  OpenAPI (AllWork publishes none). The realm AWN1 is a Keycloak deployment that\n  fronts the AllWork web application (app.allworknow.com) and the brand\n  sub-experiences (e.g. beauty.allworknow.com). No public API keys, no\n  developer-facing token issuance is documented.\nsummary:\n  types: [openIdConnect, oauth2, mutualTLS]\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n    - implicit\n    - clientCredentials\n    - password\n    - refreshToken\n    - deviceCode\n    - ciba\n    - tokenExchange\nschemes:\n  - name: allworkOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://auth.allworknow.com/realms/AWN1/.well-known/openid-configuration\n    issuer: https://auth.allworknow.com/realms/AWN1\n    sources: [well-known/allwork-openid-configuration.json]\n\
  \  - name: allworkOAuth2\n    type: oauth2\n    sources: [well-known/allwork-openid-configuration.json]\n    endpoints:\n      authorization: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth\n      token: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token\n      userinfo: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/userinfo\n      jwks: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/certs\n      end_session: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/logout\n      introspection: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token/introspect\n      revocation: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/revoke\n      device_authorization: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth/device\n      backchannel_authentication: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/ext/ciba/auth\n      pushed_authorization_request:\
  \ https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/ext/par/request\n      dynamic_client_registration: https://auth.allworknow.com/realms/AWN1/clients-registrations/openid-connect\n    grant_types_supported:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n      - urn:ietf:params:oauth:grant-type:token-exchange\n    response_types_supported:\n      - code\n      - none\n      - id_token\n      - token\n      - id_token token\n      - code id_token\n      - code token\n      - code id_token token\n    response_modes_supported:\n      - query\n      - fragment\n      - form_post\n      - query.jwt\n      - fragment.jwt\n      - form_post.jwt\n      - jwt\n    token_endpoint_auth_methods_supported:\n      - private_key_jwt\n      - client_secret_basic\n      - client_secret_post\n      - tls_client_auth\n      -\
  \ client_secret_jwt\n    code_challenge_methods_supported: [plain, S256]\n    id_token_signing_alg_values_supported:\n      [PS384, ES384, RS384, HS256, HS512, ES256, RS256, HS384, ES512, PS256, PS512, RS512]\n    subject_types_supported: [public, pairwise]\n    claims_supported:\n      [aud, sub, iss, auth_time, name, given_name, family_name, preferred_username, email, acr]\n    acr_values_supported: ['0', '1']\n    request_parameter_supported: true\n    require_pushed_authorization_requests: false\n  - name: allworkMutualTLS\n    type: mutualTLS\n    sources: [well-known/allwork-openid-configuration.json]\n    note: >-\n      tls_client_certificate_bound_access_tokens is true and mtls_endpoint_aliases\n      are advertised; tls_client_auth is an accepted client authentication method.\nobserved_in_the_wild:\n  - client_id: AWN1\n    flow: authorization_code with PKCE (S256)\n    redirect_uri: https://beauty.allworknow.com/\n    scope: openid\n    source: >-\n      login link rendered\
  \ in the public HTML of https://allworknow.com/\ngaps:\n  - No public documentation of this authorization server exists on allworknow.com.\n  - No developer key issuance, no API reference, and no documented consumer-facing token flow.\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://auth.allworknow.com/realms/AWN1/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allwork/refs/heads/main/authentication/allwork-authentication.yml
summary_line: openIdConnect/oauth2/mutualTLS · 3 schemes
tags:
- Company
- Workforce Management
- Human Resources
- Staffing
- Payroll
- Employer of Record
- Contingent Workforce
- Gig Economy
- Scheduling
- Time and Attendance
- Compliance
---
