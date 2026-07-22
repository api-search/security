---
api_key_in: []
api_specs:
- filename: remote-openapi-original.json
  format: json
  label: Remote API
  slug: remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote/refs/heads/main/openapi/remote-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Remote Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Remote secures its APIs with http and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Remote
provider_slug: remote
scheme_count: 5
schemes:
- description: 'Authenticate using the basic authentication for partners.


    Use the CLIENT_ID as login and CLIENT_SECRET as password.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/remote-openapi-original.json
  type: http
- description: 'Authenticate a partner using only the the provided `client_token`.


    This authentication method only allows accessing marketing endpoints.'
  name: ClientToken
  scheme: bearer
  sources:
  - openapi/remote-openapi-original.json
  type: http
- description: Authenticate using OAuth 2.0 protocol.
  flows:
  - authorizationUrl: /auth/oauth2/authorize
    flow: authorizationCode
    scopes: 73
    tokenUrl: /auth/oauth2/token
  - flow: clientCredentials
    scopes: 18
    tokenUrl: /auth/oauth2/token
  name: OAuth2
  sources:
  - openapi/remote-openapi-original.json
  type: oauth2
- description: Authenticate as the employee using the `urn:ietf:params:oauth:grant-type:jwt-bearer` grant in the OAuth2 protocol.
  flows:
  - flow: clientCredentials
    scopes: 21
    tokenUrl: /auth/oauth2/token
  name: OAuth2Assertion
  sources:
  - openapi/remote-openapi-original.json
  type: oauth2
- description: Authenticate as the token authorizer using `authorization_code` / `refresh_token` grants in the OAuth 2.0 protocol.
  flows:
  - authorizationUrl: /auth/oauth2/authorize
    flow: authorizationCode
    scopes: 73
    tokenUrl: /auth/oauth2/token
  name: OAuth2AuthorizationCode
  sources:
  - openapi/remote-openapi-original.json
  type: oauth2
slug: remote-authentication
source_filename: remote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/remote-openapi-original.json\ndocs: https://developer.remote.com/docs/authentication\nnotes: >-\n  Remote supports several auth methods by use case. Partners: OAuth 2.0 Client\n  Credentials (act as themselves), OAuth 2.0 Authorization Code (act on behalf\n  of a consenting customer, storing the refresh_token), OAuth 2.0 Assertion\n  (jwt-bearer, act on behalf of an employee of an authorized company), Basic\n  Auth (CLIENT_ID/CLIENT_SECRET to mint tokens), and Client Token (bearer, for\n  marketing endpoints only — no PII). Access tokens are valid for 3600 seconds.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Authenticate using the basic authentication for partners.\n\n    Use the CLIENT_ID as login and CLIENT_SECRET as password.\n  sources:\n  - openapi/remote-openapi-original.json\n\
  - name: ClientToken\n  type: http\n  scheme: bearer\n  description: |-\n    Authenticate a partner using only the the provided `client_token`.\n\n    This authentication method only allows accessing marketing endpoints.\n  sources:\n  - openapi/remote-openapi-original.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /auth/oauth2/authorize\n    tokenUrl: /auth/oauth2/token\n    scopes: 73\n  - flow: clientCredentials\n    tokenUrl: /auth/oauth2/token\n    scopes: 18\n  description: Authenticate using OAuth 2.0 protocol.\n  sources:\n  - openapi/remote-openapi-original.json\n- name: OAuth2Assertion\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/oauth2/token\n    scopes: 21\n  description: Authenticate as the employee using the `urn:ietf:params:oauth:grant-type:jwt-bearer`\n    grant in the OAuth2 protocol.\n  sources:\n  - openapi/remote-openapi-original.json\n- name: OAuth2AuthorizationCode\n  type: oauth2\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: /auth/oauth2/authorize\n    tokenUrl: /auth/oauth2/token\n    scopes: 73\n  description: Authenticate as the token authorizer using `authorization_code` / `refresh_token`\n    grants in the OAuth 2.0 protocol.\n  sources:\n  - openapi/remote-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remote/refs/heads/main/authentication/remote-authentication.yml
summary_line: http/oauth2 · 5 schemes
tags:
- Company
- HR
- Payroll
- Employer of Record
- Global Employment
- Contractors
- Benefits
- Compliance
- Human Resources
---
