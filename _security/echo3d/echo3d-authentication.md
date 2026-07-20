---
api_key_in:
- query
- body
auth_types:
- apiKey
- oidc
description: ''
kind: authentication
layout: security
method: searched
name: Echo3D Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: echo3D secures its APIs with apiKey and oidc across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: echo3D
provider_slug: echo3d
scheme_count: 5
schemes:
- description: The target collection API key (e.g. some-words-1234). Identifies the echo3D collection the request operates on. Passed as a query parameter on GET endpoints and as form-body data on POST endpoints.
  in: query
  name: CollectionKey
  parameter: key
  required: true
  sources:
  - https://docs.echo3d.com/api/queries
  type: apiKey
- description: The account email address associated with the request.
  in: query
  name: AccountEmail
  parameter: email
  required: true
  sources:
  - https://docs.echo3d.com/api/queries
  type: apiKey
- description: The personal authentication key for the account, obtained from the console Security section. Combined with key + email to authenticate API calls.
  in: query
  name: UserKey
  parameter: userKey
  required: true
  sources:
  - https://docs.echo3d.com/api/queries
  type: apiKey
- description: Optional collection secret key. Required only when secret-key protection is enabled on the collection via the console Security tab, adding a shared secret to every API call.
  in: query
  name: SecretKey
  parameter: secKey
  required: false
  sources:
  - https://docs.echo3d.com/web-console/manage-pages/collections-and-sharing/security
  type: apiKey
- description: OpenID Connect (Auth0) identity provider backing console/dashboard login and account management. Separate from the collection API-key auth used by the RESTful query API. Supports authorizationCode, clientCredentials, refreshToken and device-code grants; PKCE (S256) supported.
  issuer: https://echo3d.us.auth0.com/
  name: ConsoleOIDC
  openIdConnectUrl: https://api.echo3d.com/.well-known/openid-configuration
  sources:
  - https://api.echo3d.com/.well-known/openid-configuration
  type: openIdConnect
slug: echo3d-authentication
source_filename: echo3d-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://docs.echo3d.com/api and\n  https://api.echo3d.com/.well-known/openid-configuration\ndocs: https://docs.echo3d.com/quickstart/get-api-key\nsummary:\n  types:\n  - apiKey\n  - oidc\n  api_key_in:\n  - query\n  - body\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: CollectionKey\n  type: apiKey\n  in: query\n  parameter: key\n  required: true\n  description: >-\n    The target collection API key (e.g. some-words-1234). Identifies the echo3D\n    collection the request operates on. Passed as a query parameter on GET\n    endpoints and as form-body data on POST endpoints.\n  sources:\n  - https://docs.echo3d.com/api/queries\n- name: AccountEmail\n  type: apiKey\n  in: query\n  parameter: email\n  required: true\n  description: The account email address associated with the request.\n  sources:\n  - https://docs.echo3d.com/api/queries\n- name: UserKey\n  type: apiKey\n  in: query\n \
  \ parameter: userKey\n  required: true\n  description: >-\n    The personal authentication key for the account, obtained from the console\n    Security section. Combined with key + email to authenticate API calls.\n  sources:\n  - https://docs.echo3d.com/api/queries\n- name: SecretKey\n  type: apiKey\n  in: query\n  parameter: secKey\n  required: false\n  description: >-\n    Optional collection secret key. Required only when secret-key protection is\n    enabled on the collection via the console Security tab, adding a shared\n    secret to every API call.\n  sources:\n  - https://docs.echo3d.com/web-console/manage-pages/collections-and-sharing/security\n- name: ConsoleOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://api.echo3d.com/.well-known/openid-configuration\n  issuer: https://echo3d.us.auth0.com/\n  description: >-\n    OpenID Connect (Auth0) identity provider backing console/dashboard login and\n    account management. Separate from the collection API-key auth used by the\n\
  \    RESTful query API. Supports authorizationCode, clientCredentials,\n    refreshToken and device-code grants; PKCE (S256) supported.\n  sources:\n  - https://api.echo3d.com/.well-known/openid-configuration\nnotes: >-\n  The echo3D RESTful data API (api.echo3d.com) is authenticated with an API-key\n  triple (key + email + userKey) plus an optional collection secKey — there are\n  no OAuth scopes on the data plane. OIDC/Auth0 governs console identity only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo3d/refs/heads/main/authentication/echo3d-authentication.yml
summary_line: apiKey/oidc · 5 schemes
tags:
- Company
- 3D
- Augmented Reality
- Virtual Reality
- Digital Asset Management
- 3D Models
- Content Delivery
- Developer Tools
- SDKs
- WebAR
---
