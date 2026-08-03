---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Deepwatch Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- password
- deviceCode
overview: Deepwatch secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, password, and deviceCode flow(s).
provider_name: Deepwatch
provider_slug: deepwatch
scheme_count: 2
schemes:
- claims_count: 31
  endpoints:
    authorization: https://deepwatch.okta.com/oauth2/v1/authorize
    device_authorization: https://deepwatch.okta.com/oauth2/v1/device/authorize
    end_session: https://deepwatch.okta.com/oauth2/v1/logout
    introspection: https://deepwatch.okta.com/oauth2/v1/introspect
    jwks: https://deepwatch.okta.com/oauth2/v1/keys
    registration: https://deepwatch.okta.com/oauth2/v1/clients
    revocation: https://deepwatch.okta.com/oauth2/v1/revoke
    token: https://deepwatch.okta.com/oauth2/v1/token
    userinfo: https://deepwatch.okta.com/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg:
  - RS256
  issuer: https://deepwatch.okta.com
  name: OktaOIDC
  openIdConnectUrl: https://deepwatch.okta.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  provider: Okta
  response_types:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  sources:
  - well-known/deepwatch-openid-configuration.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- applies_to: https://devportalapi.deepwatch.com/graphql/
  name: SecurityCenterSession
  note: 'The Security Center GraphQL API (AWS AppSync) requires an authenticated session brokered by the Okta org above. Anonymous introspection is refused by a WAF rule: HTTP 403 with errorType WAFForbiddenException. No public API key, personal access token or client-credentials path is documented.'
  sources:
  - https://devportal.deepwatch.com/main.js
  transport: https
  type: session
slug: deepwatch-authentication
source_filename: deepwatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://deepwatch.okta.com/.well-known/openid-configuration\ndocs: null\ndocs_note: Deepwatch publishes no public API authentication documentation. This profile\n  is assembled from the live OIDC discovery document served by Deepwatch's Okta org\n  and from the Security Center console's own login flow and CSP.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - refreshToken\n  - password\n  - deviceCode\n  public_api: false\n  access: Authenticated Deepwatch customers only; there is no public/self-serve API\n    credential.\nschemes:\n- name: OktaOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://deepwatch.okta.com/.well-known/openid-configuration\n  issuer: https://deepwatch.okta.com\n  provider: Okta\n  sources:\n  - well-known/deepwatch-openid-configuration.json\n  endpoints:\n    authorization: https://deepwatch.okta.com/oauth2/v1/authorize\n\
  \    token: https://deepwatch.okta.com/oauth2/v1/token\n    userinfo: https://deepwatch.okta.com/oauth2/v1/userinfo\n    jwks: https://deepwatch.okta.com/oauth2/v1/keys\n    registration: https://deepwatch.okta.com/oauth2/v1/clients\n    introspection: https://deepwatch.okta.com/oauth2/v1/introspect\n    revocation: https://deepwatch.okta.com/oauth2/v1/revoke\n    end_session: https://deepwatch.okta.com/oauth2/v1/logout\n    device_authorization: https://deepwatch.okta.com/oauth2/v1/device/authorize\n  grant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types:\n  - code\n  - id_token\n  - code id_token\n  - code token\n  - id_token token\n  - code id_token token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  id_token_signing_alg:\n  -\
  \ RS256\n  subject_types:\n  - public\n  claims_count: 31\n- name: SecurityCenterSession\n  type: session\n  transport: https\n  applies_to: https://devportalapi.deepwatch.com/graphql/\n  note: 'The Security Center GraphQL API (AWS AppSync) requires an authenticated session\n    brokered by the Okta org above. Anonymous introspection is refused by a WAF rule:\n    HTTP 403 with errorType WAFForbiddenException. No public API key, personal access\n    token or client-credentials path is documented.'\n  sources:\n  - https://devportal.deepwatch.com/main.js\nobservations:\n- Okta is also named as a Deepwatch subprocessor on the trust center, consistent with\n  Okta being the identity layer for the customer console.\n- Deepwatch supports Okta and Microsoft Entra ID as customer identity data sources\n  for MDR (see legal.deepwatch.com/supported-technologies); that is a monitored data\n  source, distinct from the console's own SSO above.\nx-evidence:\n  fetched: '2026-08-01'\n  openid_configuration_http_status:\
  \ 200\n  graphql_introspection_http_status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepwatch/refs/heads/main/authentication/deepwatch-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Cybersecurity
- Managed Detection and Response
- Security Operations
- Threat Intelligence
- Vulnerability Management
- Managed Security Services
- Agentic AI
---
