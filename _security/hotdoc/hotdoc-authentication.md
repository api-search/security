---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hotdoc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: HotDoc secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: HotDoc
provider_slug: hotdoc
scheme_count: 2
schemes:
- issuer: https://www.hotdoc.com.au
  name: HotDocOpenIDConnect
  openIdConnectUrl: https://www.hotdoc.com.au/.well-known/openid-configuration
  sources:
  - well-known/hotdoc-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://www.hotdoc.com.au/oauth/authorize
    flow: authorizationCode
    scopes:
      openid: OpenID Connect authentication
    tokenUrl: https://www.hotdoc.com.au/oauth/token
  - authorizationUrl: https://www.hotdoc.com.au/oauth/authorize
    flow: implicit
    scopes:
      openid: OpenID Connect authentication
  name: HotDocOAuth2
  sources:
  - well-known/hotdoc-oauth-authorization-server.json
  type: oauth2
slug: hotdoc-authentication
source_filename: hotdoc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://www.hotdoc.com.au/.well-known/openid-configuration\nnote: >-\n  Derived from HotDoc's live OpenID Connect / OAuth 2.0 Authorization Server\n  Metadata (RFC 8414 + OpenID Connect Discovery 1.0), served as real JSON on both\n  the www and api hosts. There is no published OpenAPI, so this profile is taken\n  directly from the discovery document rather than from securitySchemes. The\n  authorization server is a Rails/Doorkeeper deployment; access is\n  partner/clinic-gated (no self-serve developer client registration is\n  documented).\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  api_key_in: []\nschemes:\n- name: HotDocOpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.hotdoc.com.au/.well-known/openid-configuration\n  issuer: https://www.hotdoc.com.au\n  sources:\n  - well-known/hotdoc-openid-configuration.json\n- name: HotDocOAuth2\n  type:\
  \ oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.hotdoc.com.au/oauth/authorize\n    tokenUrl: https://www.hotdoc.com.au/oauth/token\n    scopes:\n      openid: OpenID Connect authentication\n  - flow: implicit\n    authorizationUrl: https://www.hotdoc.com.au/oauth/authorize\n    scopes:\n      openid: OpenID Connect authentication\n  sources:\n  - well-known/hotdoc-oauth-authorization-server.json\nendpoints:\n  authorization: https://www.hotdoc.com.au/oauth/authorize\n  token: https://www.hotdoc.com.au/oauth/token\n  userinfo: https://www.hotdoc.com.au/oauth/userinfo\n  introspection: https://www.hotdoc.com.au/oauth/introspect\n  revocation: https://www.hotdoc.com.au/oauth/revoke\n  jwks: https://www.hotdoc.com.au/oauth/discovery/keys\ntoken_endpoint_auth_methods:\n- client_secret_basic\n- client_secret_post\nid_token_signing_alg: RS256\nsubject_types:\n- pairwise\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- email\n- given_name\n- family_name\n\
  - full_name\n- practice_name\n- pms_software\n- access_level\n- company\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotdoc/refs/heads/main/authentication/hotdoc-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Healthcare
- Australia
- Patient Engagement
- Online Booking
- Appointment Scheduling
- Telehealth
- Practice Management
- Primary Care
- Digital Health
- e-Prescribing
---
