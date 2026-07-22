---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Everysim Inc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- deviceCode
overview: EverySim Inc. secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, and deviceCode flow(s).
provider_name: EverySim Inc.
provider_slug: everysim-inc
scheme_count: 2
schemes:
- issuer: https://auth.everysim.io/realms/everysim
  name: openIdConnect
  openIdConnectUrl: https://auth.everysim.io/realms/everysim/.well-known/openid-configuration
  sources:
  - well-known/everysim-inc-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/auth
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    pkce: true
    tokenUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/token
  name: oauth2
  type: oauth2
slug: everysim-inc-authentication
source_filename: everysim-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://auth.everysim.io/realms/everysim/.well-known/openid-configuration\ndocs: https://auth.everysim.io/realms/everysim/.well-known/openid-configuration\nnotes: >-\n  Derived from EverySim's live OpenID Connect discovery document (Keycloak,\n  realm \"everysim\"). No public OpenAPI is available, so this profile is\n  captured directly from the provider's IdP configuration. The everysim.io\n  web app authenticates the \"everysim-web\" client via authorization-code + PKCE.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - password\n  - deviceCode\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.everysim.io/realms/everysim/.well-known/openid-configuration\n  issuer: https://auth.everysim.io/realms/everysim\n  sources:\n  - well-known/everysim-inc-openid-configuration.json\n- name: oauth2\n  type: oauth2\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/auth\n    tokenUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/token\n    pkce: true\n    code_challenge_methods:\n    - S256\n    - plain\n  - flow: clientCredentials\n    tokenUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/token\nendpoints:\n  authorization: https://auth.everysim.io/realms/everysim/protocol/openid-connect/auth\n  token: https://auth.everysim.io/realms/everysim/protocol/openid-connect/token\n  userinfo: https://auth.everysim.io/realms/everysim/protocol/openid-connect/userinfo\n  introspection: https://auth.everysim.io/realms/everysim/protocol/openid-connect/token/introspect\n  end_session: https://auth.everysim.io/realms/everysim/protocol/openid-connect/logout\n  jwks_uri: https://auth.everysim.io/realms/everysim/protocol/openid-connect/certs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everysim-inc/refs/heads/main/authentication/everysim-inc-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Authentication
- OpenID Connect
- OAuth 2.0
- Single Sign-On
- Identity
---
