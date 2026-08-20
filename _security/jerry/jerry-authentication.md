---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Jerry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jerry secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jerry
provider_slug: jerry
scheme_count: 1
schemes:
- discovery_completeness: minimal
  id_token_signing_alg_values_supported:
  - RS256
  interpretation: Only the implicit `id_token` response type is advertised and no token or authorization endpoint is published, so no authorization-code + PKCE flow is discoverable. There is no third-party client registration path and no scope vocabulary, so `scopes/` is intentionally not emitted for this provider.
  issuer: https://getjerry.com
  jwks_uri: https://getjerry.com/.well-known/jwks.json
  missing_from_discovery:
  - authorization_endpoint
  - token_endpoint
  - userinfo_endpoint
  - registration_endpoint
  - scopes_supported
  - grant_types_supported
  - claims_supported
  - code_challenge_methods_supported
  name: OpenIDConnect
  openIdConnectUrl: https://getjerry.com/.well-known/openid-configuration
  response_types_supported:
  - id_token
  sources:
  - well-known/jerry-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
slug: jerry-authentication
source_filename: jerry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://getjerry.com/.well-known/openid-configuration\ndocs: null\nsummary:\n  types: [openIdConnect]\n  api_key_in: []\n  oauth2_flows: []\n  public_api: false\n  note: >-\n    Jerry publishes no public developer API and no developer authentication\n    documentation. This profile is derived entirely from the one authentication\n    artifact Jerry actually serves anonymously: an OpenID Connect discovery\n    document. It describes how Jerry's own first-party clients verify identity\n    tokens; it is not an authorization server third parties can register with.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://getjerry.com/.well-known/openid-configuration\n  sources: [well-known/jerry-openid-configuration.json]\n  issuer: https://getjerry.com\n  jwks_uri: https://getjerry.com/.well-known/jwks.json\n  response_types_supported: [id_token]\n  subject_types_supported: [public]\n  id_token_signing_alg_values_supported:\
  \ [RS256]\n  discovery_completeness: minimal\n  missing_from_discovery:\n  - authorization_endpoint\n  - token_endpoint\n  - userinfo_endpoint\n  - registration_endpoint\n  - scopes_supported\n  - grant_types_supported\n  - claims_supported\n  - code_challenge_methods_supported\n  interpretation: >-\n    Only the implicit `id_token` response type is advertised and no token or\n    authorization endpoint is published, so no authorization-code + PKCE flow is\n    discoverable. There is no third-party client registration path and no scope\n    vocabulary, so `scopes/` is intentionally not emitted for this provider.\ngaps:\n- No developer portal, API reference or authentication documentation is published.\n- No API keys, bearer-token, or OAuth 2.0 client credentials surface is documented.\n- Discovery omits authorization_endpoint / token_endpoint, so the OIDC document is\n  not usable by a third-party relying party as published.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://getjerry.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jerry/refs/heads/main/authentication/jerry-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Auto Insurance
- Insurance Broker
- Automotive
- Consumer Finance
- Lending
- Telematics
- Mobile Applications
- Artificial Intelligence
---
