---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Electronic Arts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electronic Arts declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Electronic Arts
provider_slug: electronic-arts
scheme_count: 0
schemes: []
slug: electronic-arts-authentication
source_filename: electronic-arts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://accounts.ea.com/.well-known/openid-configuration (HTTP 200) and\n  https://accounts.ea.com/.well-known/oauth-authorization-server (HTTP 200), both fetched\n  2026-09-06 and saved verbatim to well-known/; enriched from EA's own FC Community API\n  announcement at https://www.ea.com/games/ea-sports-fc/fc-26/news/pitch-notes-fc26-community-api-update\n  (HTTP 200) and https://help.ea.com/en/articles/ea-sports-fc/community-api/ (HTTP 200).\nprovider: Electronic Arts\nproviderId: electronic-arts\nsummary: >-\n  Electronic Arts publishes no OpenAPI, so this profile is read from the OpenID Connect\n  Discovery and RFC 8414 authorization-server metadata EA actually serves on\n  accounts.ea.com. Every EA integration surface known to be public — the EA app, the\n  approved EA SPORTS FC community partners — authenticates through this one authorization\n  server. There is no public API-key programme and no self-service client\
  \ registration.\nauthorization_server:\n  issuer: accounts.ea.com\n  authorization_endpoint: https://accounts.ea.com/connect/auth\n  token_endpoints:\n  - https://accounts.ea.com/connect/token\n  - https://accounts2s.ea.com/connect/token\n  - https://accounts.internal.ea.com/connect/token\n  userinfo_endpoint: https://accounts.ea.com/connect/userinfo\n  jwks_uri: https://accounts.ea.com/connect/.well-known/openid-configuration/certs\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_certificate_post\n  subject_types_supported:\n  - public\nsecurity_schemes:\n- name: ea_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://accounts.ea.com/.well-known/openid-configuration\n  description: >-\n    EA Account OpenID Connect. Advertises the full response_types matrix\n    (code, token, id_token and every hybrid combination), RS256-signed ID tokens, and\
  \ the\n    openid/email/phone/profile scope set. Client credentials are issued by EA; there is no\n    public registration endpoint and the discovery document advertises none.\n- name: ea_oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://accounts.ea.com/connect/auth\n  tokenUrl: https://accounts.ea.com/connect/token\n  pkce: supported\n  description: >-\n    The delegated-consent flow behind the EA SPORTS FC Community API. EA's own wording:\n    the player completes \"a secure EA login flow\", is \"asked to grant that website\n    permission to make specific requests to FC services on your behalf\", and the partner\n    site receives \"permissions to make specific API requests\" but never the password or\n    login credentials.\n- name: ea_mtls_client\n  type: mutualTLS\n  description: >-\n    client_certificate_post is advertised as a token-endpoint client authentication method\n    alongside client_secret_post, implying certificate-bound\
  \ partner clients. EA publishes\n    no documentation for it; recorded because the discovery document declares it.\nclient_onboarding:\n  self_service: false\n  public_registration_endpoint: false\n  process: >-\n    Partner approval only. EA states plainly on the FC Community API announcement: \"We are\n    not accepting requests at this time.\" The three approved EA SPORTS FC community\n    partners at the time of this probe are FUT.GG, FUTBIN and FUTWIZ.\n  source: https://www.ea.com/games/ea-sports-fc/fc-26/news/pitch-notes-fc26-community-api-update\ngaps:\n- >-\n  No public API reference, no scope reference beyond the four OIDC scopes in the discovery\n  document, and no documented base URL for the FC Community API resource server.\n- >-\n  No /.well-known/oauth-protected-resource (RFC 9728) is served on any EA host, so a client\n  cannot discover which resource server the tokens are for.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electronic-arts/refs/heads/main/authentication/electronic-arts-authentication.yml
summary_line: 0 schemes
tags:
- Gaming
- Video Games
- Entertainment
- Consumer
- Player Services
- Fortune 1000
---
