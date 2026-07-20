---
api_key_in: []
api_specs:
- filename: ccp-games-esi-openapi-original.json
  format: json
  label: EVE Swagger Interface (ESI)
  slug: eve-swagger-interface-esi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ccp-games/refs/heads/main/openapi/ccp-games-esi-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ccp Games Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CCP Games secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CCP Games
provider_slug: ccp-games
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.eveonline.com/v2/oauth/authorize
    flow: authorizationCode
    scopes: 70
    tokenUrl: https://login.eveonline.com/v2/oauth/token
  name: OAuth2
  sources:
  - openapi/ccp-games-esi-openapi-original.json
  type: oauth2
slug: ccp-games-authentication
source_filename: ccp-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/ccp-games-esi-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  scheme_names:\n  - EVE SSO (OAuth 2.0 / OpenID Connect)\n  oidc: true\n  pkce: S256\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.eveonline.com/v2/oauth/authorize\n    tokenUrl: https://login.eveonline.com/v2/oauth/token\n    scopes: 70\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\ndocs: https://docs.esi.evetech.net/docs/sso/\ndiscovery:\n  oauth_authorization_server: https://login.eveonline.com/.well-known/oauth-authorization-server\n  openid_configuration: https://login.eveonline.com/.well-known/openid-configuration\n  jwks_uri: https://login.eveonline.com/oauth/jwks\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccp-games/refs/heads/main/authentication/ccp-games-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Gaming
- Games
- MMO
- EVE Online
- Developer Platform
- OAuth
- OpenID Connect
- Player Data
- Virtual Economy
---
