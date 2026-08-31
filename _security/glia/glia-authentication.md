---
api_key_in:
- body
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Glia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glia secures its APIs with http and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Glia
provider_slug: glia
scheme_count: 4
schemes:
- description: The primary scheme for platform/management API calls. The 401 body on GET /operators names the requirement explicitly ("Authorization header must have format 'token_type token'").
  format: 'Authorization: Bearer <token>'
  in: header
  name: bearerToken
  parameter: Authorization
  scheme: bearer
  sources:
  - probe:https://api.glia.com/sites
  - src/lib/api.js
  type: http
- description: Visitor/engagement endpoints accept two additional token types. GET /engagements returns "Authorization header must have format 'token_type token' where token_type is SessionId or AuthToken", i.e. visitor session identifiers and visitor auth tokens are first-class credential types alongside operator bearer tokens.
  format: 'Authorization: <SessionId|AuthToken> <token>'
  in: header
  name: sessionOrAuthToken
  parameter: Authorization
  scheme: custom
  sources:
  - probe:https://api.glia.com/engagements
  type: http
- description: Site-scoped API key id and secret exchanged for a bearer token. Distributed to integrators as GLIA_KEY_ID / GLIA_KEY_SECRET alongside a GLIA_SITE_ID.
  in: body
  name: apiKeyPair
  parameters:
  - api_key_id
  - api_key_secret
  sources:
  - src/lib/config.js
  type: apiKey
- description: POST /operator_authentication/tokens with an empty body returns 422 {"details":[{"attribute":"api_token","detail":"must be present"}]}, so the endpoint also accepts an api_token attribute directly.
  in: body
  name: operatorApiToken
  parameters:
  - api_token
  sources:
  - probe:https://api.glia.com/operator_authentication/tokens
  type: apiKey
slug: glia-authentication
source_filename: glia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: >-\n  live probes of api.glia.com/api.glia.eu plus the first-party client in\n  salemove/glia-functions-tools (src/lib/api.js, src/lib/config.js)\ndocs: https://docs.glia.com/glia-dev\ndocs_access: gated\nsummary:\n  types: [http, apiKey]\n  api_key_in: [body]\n  oauth2_flows: []\n  note: >-\n    Glia does not expose OAuth 2.0 or OpenID Connect discovery on any host probed. The model is a\n    two-step exchange: a long-lived API key id/secret pair is posted to a token endpoint, which\n    returns a short-lived bearer token presented on every subsequent request. Derived from a\n    published spec is not possible - Glia publishes no OpenAPI - so this profile is assembled\n    from observed HTTP responses and first-party client source.\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <token>'\n  description: >-\n    The primary scheme for platform/management\
  \ API calls. The 401 body on GET /operators names\n    the requirement explicitly (\"Authorization header must have format 'token_type token'\").\n  sources: [probe:https://api.glia.com/sites, src/lib/api.js]\n- name: sessionOrAuthToken\n  type: http\n  scheme: custom\n  in: header\n  parameter: Authorization\n  format: 'Authorization: <SessionId|AuthToken> <token>'\n  description: >-\n    Visitor/engagement endpoints accept two additional token types. GET /engagements returns\n    \"Authorization header must have format 'token_type token' where token_type is SessionId or\n    AuthToken\", i.e. visitor session identifiers and visitor auth tokens are first-class\n    credential types alongside operator bearer tokens.\n  sources: [probe:https://api.glia.com/engagements]\n- name: apiKeyPair\n  type: apiKey\n  in: body\n  parameters: [api_key_id, api_key_secret]\n  description: >-\n    Site-scoped API key id and secret exchanged for a bearer token. Distributed to integrators as\n    GLIA_KEY_ID\
  \ / GLIA_KEY_SECRET alongside a GLIA_SITE_ID.\n  sources: [src/lib/config.js]\n- name: operatorApiToken\n  type: apiKey\n  in: body\n  parameters: [api_token]\n  description: >-\n    POST /operator_authentication/tokens with an empty body returns 422\n    {\"details\":[{\"attribute\":\"api_token\",\"detail\":\"must be present\"}]}, so the endpoint also\n    accepts an api_token attribute directly.\n  sources: [probe:https://api.glia.com/operator_authentication/tokens]\nendpoints:\n- purpose: mint bearer token\n  method: POST\n  url: https://api.glia.com/operator_authentication/tokens\n  request: {api_key_id: string, api_key_secret: string}\n  observed_status: 422\n  observed_body: '{\"details\":[{\"attribute\":\"api_token\",\"detail\":\"must be present\"}],\"error\":\"validation_error\",\"status\":\"error\"}'\n- purpose: validate current session\n  method: GET\n  url: https://api.glia.com/operator_authentication/sessions/current\n  auth: Bearer\n  source: src/lib/config.js\ndeprecations:\n\
  - credential: Site API key\n  superseded_by: service credentials API key authentication\n  announced: '2026-02-17'\n  source: https://github.com/salemove/android-sdk-widgets/releases/tag/3.5.0\n  note: >-\n    Glia introduced \"service credentials\" to align service-to-service API keys with its access\n    management framework and marked the site API key deprecated in the same release. No sunset\n    date is published.\ntoken_lifecycle:\n  expiry: true\n  expiry_field: token expiry tracked client-side (GLIA_TOKEN_EXPIRES_AT)\n  refresh: >-\n    The first-party client re-mints a token from the key pair when the current one is within five\n    minutes of expiry; there is no refresh_token grant.\n  revocation_docs: null\nregions:\n- {region: Americas, host: https://api.glia.com}\n- {region: EU, host: https://api.glia.eu}\n- {region: legacy, host: https://api.salemove.com}\n- {region: beta, host: https://api.beta.glia.com}\nnot_found:\n  oauth2: 'GET /oauth/token -> 404; no /.well-known/oauth-authorization-server'\n\
  \  openid_connect: 'no /.well-known/openid-configuration'\n  jwks: 'GET /.well-known/jwks.json -> 404'\n  mtls: not documented publicly\nx-evidence:\n- {url: 'https://api.glia.com/operators', http_status: 401, fetched: '2026-08-04'}\n- {url: 'https://api.glia.com/sites', http_status: 401, fetched: '2026-08-04'}\n- {url: 'https://api.glia.com/engagements', http_status: 401, fetched: '2026-08-04'}\n- {url: 'https://api.glia.com/operator_authentication/tokens', http_status: 422, fetched: '2026-08-04'}\n- {url: 'https://github.com/salemove/glia-functions-tools/blob/main/src/lib/config.js', http_status: 200, fetched: '2026-08-04'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glia/refs/heads/main/authentication/glia-authentication.yml
summary_line: http/apiKey · 4 schemes
tags:
- Company
- Customer Service
- Contact Center
- Banking
- Credit Unions
- Financial-Services
- Conversational AI
- Voice
- CoBrowsing
- Serverless
---
