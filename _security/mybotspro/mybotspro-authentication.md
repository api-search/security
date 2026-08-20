---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Mybotspro Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- refreshToken
overview: Mybots.pro secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, and refreshToken flow(s).
provider_name: Mybots.pro
provider_slug: mybotspro
scheme_count: 3
schemes:
- issuer: https://auth.mybots.pro/
  name: OpenIDConnect
  openIdConnectUrl: https://auth.mybots.pro/.well-known/openid-configuration
  source: well-known/mybotspro-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.mybots.pro/connect/authorize
    flow: authorizationCode
    refreshUrl: https://auth.mybots.pro/connect/token
    tokenUrl: https://auth.mybots.pro/connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.mybots.pro/connect/token
  - flow: password
    note: Resource-owner password credentials is advertised in grant_types_supported. OAuth 2.1 deprecates this grant; recorded because the provider advertises it, not endorsed.
    tokenUrl: https://auth.mybots.pro/connect/token
  name: OAuth2
  source: well-known/mybotspro-openid-configuration.json
  type: oauth2
- evidence:
    header: 'www-authenticate: Bearer'
    http_status: 401
    observed: '2026-08-14'
    url: https://client.mybots.pro/api/Subscribe/program
  name: BearerToken
  scheme: bearer
  source: observed response header
  type: http
slug: mybotspro-authentication
source_filename: mybotspro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://auth.mybots.pro/.well-known/openid-configuration\nnote: >-\n  Derived from the provider's OWN live OAuth 2.0 / OpenID Connect discovery document, not\n  from an OpenAPI — myBots publishes no OpenAPI anywhere (see conformance/ for the full\n  negative probe record). Every value below is copied verbatim from that document or was\n  observed on a live response; nothing is inferred. The server is OpenIddict (identified by\n  the error_uri documentation.openiddict.com returned by the token endpoint).\ndocs: null\ndocs_note: >-\n  myBots publishes no developer authentication guide. The discovery document IS the only\n  machine-readable auth contract they serve.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, password, refreshToken]\n  bearer: true\n  pkce: true\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.mybots.pro/.well-known/openid-configuration\n\
  \  issuer: https://auth.mybots.pro/\n  source: well-known/mybotspro-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  source: well-known/mybotspro-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mybots.pro/connect/authorize\n    tokenUrl: https://auth.mybots.pro/connect/token\n    refreshUrl: https://auth.mybots.pro/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.mybots.pro/connect/token\n  - flow: password\n    tokenUrl: https://auth.mybots.pro/connect/token\n    note: >-\n      Resource-owner password credentials is advertised in grant_types_supported. OAuth 2.1\n      deprecates this grant; recorded because the provider advertises it, not endorsed.\n- name: BearerToken\n  type: http\n  scheme: bearer\n  source: observed response header\n  evidence:\n    url: https://client.mybots.pro/api/Subscribe/program\n    http_status: 401\n    header: 'www-authenticate: Bearer'\n    observed: '2026-08-14'\nendpoints:\n\
  \  authorization: https://auth.mybots.pro/connect/authorize\n  token: https://auth.mybots.pro/connect/token\n  introspection: https://auth.mybots.pro/connect/introspect\n  userinfo: https://auth.mybots.pro/connect/userinfo\n  end_session: https://auth.mybots.pro/connect/logout\n  jwks: https://auth.mybots.pro/.well-known/jwks\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- password\n- refresh_token\n- verification_token\n- session_token\nnon_standard_grants:\n- grant: verification_token\n  note: >-\n    Not an IANA-registered OAuth grant type. Undocumented by myBots; almost certainly the\n    phone/email verification exchange the SPA drives via /api/verification.\n- grant: session_token\n  note: Not an IANA-registered OAuth grant type. Undocumented by myBots.\ntoken_endpoint_auth_methods_supported:\n- client_secret_post\n- private_key_jwt\n- client_secret_basic\ncode_challenge_methods_supported: [plain, S256]\npkce_note: >-\n  S256 is supported, but so is `plain`,\
  \ which PKCE (RFC 7636 §7.2) and OAuth 2.1 both\n  discourage; a client that negotiates `plain` gets no real protection.\nid_token_signing_alg_values_supported: [RS256]\nresponse_types_supported: [code]\nresponse_modes_supported: [query, form_post, fragment]\nsubject_types_supported: [public]\nprompt_values_supported: [consent, login, none, select_account]\nsecurity_posture:\n  require_pushed_authorization_requests: false\n  claims_parameter_supported: false\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\n  tls_client_certificate_bound_access_tokens: false\n  authorization_response_iss_parameter_supported: true\nanonymous_surface:\n- api: myBots Web Chat Public API\n  endpoint: https://notification.mybots.pro/api/IntegrationApp/public/webchat/{channel}/config\n  auth: none\n  note: >-\n    Called by the published widget loader with `credentials: \"omit\"`. The channel public key\n    in the URL is the only identifier; the backend enforces a per-channel\
  \ domain allow-list\n    against the embedding page origin instead of a token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mybotspro/refs/heads/main/authentication/mybotspro-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- AI Agents
- Conversational AI
- Messaging
- Chatbots
- Customer-Support
- Sales Automation
- WhatsApp
- Telegram
- Instagram
- Omnichannel
- Lead Qualification
- OpenID Connect
---
