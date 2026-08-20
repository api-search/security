---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Easywebinar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- implicit
overview: EasyWebinar secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and implicit flow(s).
provider_name: EasyWebinar
provider_slug: easywebinar
scheme_count: 2
schemes:
- issuer: https://app.easywebinar.com
  name: EasyWebinarOIDC
  openIdConnectUrl: https://app.easywebinar.com/.well-known/openid-configuration
  sources:
  - well-known/easywebinar-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://app.easywebinar.com/oauth/authorize/
    flow: authorizationCode
    refreshUrl: https://app.easywebinar.com/oauth/token/
    scopes:
    - openid
    - profile
    - email
    - basic
    tokenUrl: https://app.easywebinar.com/oauth/token/
  - flow: clientCredentials
    scopes:
    - openid
    - profile
    - email
    - basic
    tokenUrl: https://app.easywebinar.com/oauth/token/
  - authorizationUrl: https://app.easywebinar.com/oauth/authorize/
    flow: implicit
    scopes:
    - openid
    - profile
    - email
    - basic
  name: EasyWebinarOAuth2
  sources:
  - well-known/easywebinar-oauth-authorization-server.json
  type: oauth2
slug: easywebinar-authentication
source_filename: easywebinar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://app.easywebinar.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Derived from the live OpenID Connect / RFC 8414 discovery document EasyWebinar serves at\n  app.easywebinar.com — there is no public authentication reference page. The EasyWebinar\n  REST API itself is a paid entitlement (Scale plan and Enterprise), and no public\n  documentation of its auth model exists, so everything below is what the authorization\n  server itself publishes plus what its endpoints returned to anonymous probes.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, implicit]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\nschemes:\n  - name: EasyWebinarOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://app.easywebinar.com/.well-known/openid-configuration\n    issuer: https://app.easywebinar.com\n \
  \   sources: [well-known/easywebinar-openid-configuration.json]\n  - name: EasyWebinarOAuth2\n    type: oauth2\n    sources: [well-known/easywebinar-oauth-authorization-server.json]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.easywebinar.com/oauth/authorize/\n        tokenUrl: https://app.easywebinar.com/oauth/token/\n        refreshUrl: https://app.easywebinar.com/oauth/token/\n        scopes: [openid, profile, email, basic]\n      - flow: clientCredentials\n        tokenUrl: https://app.easywebinar.com/oauth/token/\n        scopes: [openid, profile, email, basic]\n      - flow: implicit\n        authorizationUrl: https://app.easywebinar.com/oauth/authorize/\n        scopes: [openid, profile, email, basic]\nendpoints:\n  authorization: https://app.easywebinar.com/oauth/authorize/\n  token: https://app.easywebinar.com/oauth/token/\n  userinfo: https://app.easywebinar.com/oauth/me/\n  introspection: https://app.easywebinar.com/oauth/introspection/\n\
  \  revocation: https://app.easywebinar.com/oauth/revoke/\n  end_session: https://app.easywebinar.com/oauth/destroy/\n  jwks: https://app.easywebinar.com/.well-known/keys/\n  registration: null\ngrant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - uswo_me_resource_returner_credentials\n  - implicit\nresponse_types_supported: [code, id_token, token id_token, code id_token]\nsubject_types_supported: [public]\ndeviations:\n  - id: no-dynamic-registration\n    detail: registration_endpoint is explicitly null — clients must be provisioned out of band.\n  - id: no-service-documentation\n    detail: service_documentation is null; the discovery document points at no human reference.\n  - id: implicit-flow-advertised\n    detail: >-\n      The implicit grant and the \"token id_token\" response type are still advertised;\n      OAuth 2.1 / BCP 225 deprecate implicit for public clients.\n  - id: single-client-auth-method\n    detail: only client_secret_basic\
  \ is advertised — no client_secret_post, no PKCE/S256 announcement.\n  - id: no-code-challenge-methods\n    detail: code_challenge_methods_supported is absent from the discovery document, so PKCE support is unstated.\n  - id: nonstandard-grant-type\n    detail: >-\n      \"uswo_me_resource_returner_credentials\" is a vendor-private grant type (the uswo_\n      prefix belongs to the WP OAuth Server implementation) and is not documented anywhere public.\n  - id: empty-jwks-key-material\n    detail: >-\n      The JWKS at /.well-known/keys/ returns one RS256 key with n and e as empty strings,\n      so an id_token cannot be verified from the published metadata.\nsso:\n  saml2: true\n  scim: true\n  two_factor: true\n  availability: Enterprise plan only\n  source: https://easywebinar.com/enterprise/\nx-evidence:\n  - url: https://app.easywebinar.com/.well-known/openid-configuration\n    status: 200\n  - url: https://app.easywebinar.com/.well-known/oauth-authorization-server\n    status: 200\n\
  \  - url: https://app.easywebinar.com/.well-known/keys/\n    status: 200\n  - url: https://app.easywebinar.com/oauth/authorize/\n    status: 400\n    body: '{\"error\":\"invalid_client\",\"error_description\":\"No client id supplied\"}'\n  - url: https://app.easywebinar.com/oauth/token/\n    status: 405\n    body: request method must be POST when requesting an access token\n  - url: https://app.easywebinar.com/oauth/me/\n    status: 400\n    body: '{\"error\":\"invalid_request\",\"error_description\":\"Invalid token\"}'\n  - url: https://easywebinar.com/enterprise/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easywebinar/refs/heads/main/authentication/easywebinar-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Webinars
- Video
- Live Streaming
- Marketing
- Event
- CRM
- Lead Generation
- Automation
- Identity
- Authentication
- Software-as-a-Service
---
