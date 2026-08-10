---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Everly Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
- refreshToken
overview: Everly Health secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, password, and refreshToken flow(s).
provider_name: Everly Health
provider_slug: everly-health
scheme_count: 2
schemes:
- issuer: https://secure.everlywell.com
  name: openIdConnect
  openIdConnectUrl: https://secure.everlywell.com/.well-known/openid-configuration
  sources:
  - well-known/everly-health-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://secure.everlywell.com/oauth2/authorize
    flow: authorizationCode
    scopes:
      openid: OpenID Connect authentication
      public: Public scope declared by the authorization server
    tokenUrl: https://secure.everlywell.com/oauth2/token
  - flow: password
    note: The resource owner password credentials grant is declared in grant_types_supported. OAuth 2.1 and RFC 9700 (BCP) deprecate this grant; it is recorded here because the server advertises it, not as a recommendation.
    tokenUrl: https://secure.everlywell.com/oauth2/token
  issuer: https://secure.everlywell.com
  name: oauth2
  sources:
  - well-known/everly-health-oauth-authorization-server.json
  type: oauth2
slug: everly-health-authentication
source_filename: everly-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://secure.everlywell.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Everly Health publishes no developer authentication documentation. This profile was\n  read entirely from the anonymously served OpenID Connect Discovery / RFC 8414\n  document on the member login host. Nothing here is derived from an OpenAPI — the\n  company publishes none — and nothing is inferred beyond what the discovery document\n  literally declares.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - password\n  - refreshToken\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://secure.everlywell.com/.well-known/openid-configuration\n  issuer: https://secure.everlywell.com\n  sources:\n  - well-known/everly-health-openid-configuration.json\n- name: oauth2\n  type: oauth2\n  issuer: https://secure.everlywell.com\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.everlywell.com/oauth2/authorize\n    tokenUrl: https://secure.everlywell.com/oauth2/token\n    scopes:\n      openid: OpenID Connect authentication\n      public: Public scope declared by the authorization server\n  - flow: password\n    tokenUrl: https://secure.everlywell.com/oauth2/token\n    note: >-\n      The resource owner password credentials grant is declared in\n      grant_types_supported. OAuth 2.1 and RFC 9700 (BCP) deprecate this grant; it is\n      recorded here because the server advertises it, not as a recommendation.\n  sources:\n  - well-known/everly-health-oauth-authorization-server.json\nendpoints:\n  authorization: https://secure.everlywell.com/oauth2/authorize\n  token: https://secure.everlywell.com/oauth2/token\n  revocation: https://secure.everlywell.com/oauth2/revoke\n  introspection: https://secure.everlywell.com/oauth2/introspect\n  userinfo: https://secure.everlywell.com/oauth2/userinfo\n\
  \  jwks: https://secure.everlywell.com/jwks/signature\ntoken_endpoint_auth_methods:\n- client_secret_basic\n- client_secret_post\nresponse_types:\n- code\nresponse_modes:\n- query\n- fragment\n- form_post\nsubject_types:\n- public\nid_token_signing_alg:\n- RS256\nclaims:\n- iss\n- sub\n- aud\n- exp\n- iat\n- name\n- email\ngaps:\n- No public developer portal, API reference, or authentication guide.\n- No client registration endpoint advertised (no RFC 7591 dynamic registration).\n- No /.well-known/oauth-protected-resource (RFC 9728), so no resource-server metadata.\n- Only two scopes declared (openid, public) — no granular resource scopes.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://secure.everlywell.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everly-health/refs/heads/main/authentication/everly-health-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Health
- Healthcare
- Digital Health
- Diagnostics
- Lab Testing
- Telehealth
- Consumer Health
- Identity
---
