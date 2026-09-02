---
api_key_in: []
api_specs:
- filename: frayt-match-estimates-api-openapi.yml
  format: yaml
  label: FRAYT match estimates API
  slug: frayt-match-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frayt/refs/heads/main/openapi/frayt-match-estimates-api-openapi.yml
- filename: frayt-matches-api-openapi.yml
  format: yaml
  label: FRAYT Matches API
  slug: frayt-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frayt/refs/heads/main/openapi/frayt-matches-api-openapi.yml
- filename: frayt-oauth-api-openapi.yml
  format: yaml
  label: FRAYT OAUTH API
  slug: frayt-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frayt/refs/heads/main/openapi/frayt-oauth-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Frayt Authentication
name_suffix: Authentication
oauth_flows: []
overview: FRAYT secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FRAYT
provider_slug: frayt
scheme_count: 1
schemes:
- applied_to: all operations except POST /api/v2.2/oauth/token
  description: Bearer token obtained from the FRAYT token endpoint.
  format: Bearer <token>
  header: Authorization
  name: authorization
  scheme: bearer
  sources:
  - openapi/frayt-match-estimates-openapi.yml
  - openapi/frayt-matches-openapi.yml
  - openapi/frayt-oauth-openapi.yml
  type: http
slug: frayt-authentication
source_filename: frayt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\ndocs: https://api.frayt.com/docs/api/v2.2\nsource: >-\n  openapi/frayt-matches-openapi.yml, openapi/frayt-match-estimates-openapi.yml,\n  openapi/frayt-oauth-openapi.yml, plus the Authentication section of the FRAYT\n  Client API documentation and live probes of the token endpoint.\nnote: >-\n  FRAYT names its token endpoint \"oauth\" and its docs call the mechanism OAuth, but\n  it is NOT RFC 6749 and the OpenAPI itself does not declare an `oauth2`\n  securityScheme — the only scheme in the spec is `http`/`bearer`. The token\n  exchange is a proprietary JSON POST. Because there is no oauth2 scheme and no\n  scopes anywhere in the spec or docs, NO scopes/ artifact and no `OAuthScopes`\n  pointer were written for this provider; derive-oauth-scopes.py confirmed zero\n  oauth2 schemes and zero scopes.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  scopes_published: false\n  self_service_signup:\
  \ false\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the FRAYT token endpoint.\n  header: Authorization\n  format: 'Bearer <token>'\n  applied_to: all operations except POST /api/v2.2/oauth/token\n  sources:\n  - openapi/frayt-match-estimates-openapi.yml\n  - openapi/frayt-matches-openapi.yml\n  - openapi/frayt-oauth-openapi.yml\ntoken_exchange:\n  operation: FraytElixirWeb.API.OauthController.authenticate\n  endpoint: POST https://api.frayt.com/api/v2.2/oauth/token\n  sandbox_endpoint: POST https://sandbox.api.frayt.com/api/v2.2/oauth/token\n  request_media_type: application/json\n  request_schema: Oauth Request\n  request_fields:\n  - {name: client_id, required: true, description: Client ID issued by FRAYT}\n  - {name: secret, required: false, description: Secret key (optional if client_secret is present)}\n  - {name: client_secret, required: false, description: Client secret (optional if secret is present)}\n  response_schema:\
  \ Oauth Response\n  response_shape: '{\"response\": {\"token\": \"<bearer token>\"}}'\n  rfc6749_compliant: false\n  deviations:\n  - No `grant_type` parameter; the grant is implicit.\n  - Request body is JSON, not application/x-www-form-urlencoded.\n  - 'Response is `{response: {token}}`, not `{access_token, token_type, expires_in}`.'\n  - No `expires_in` is returned, so token lifetime is undiscoverable from the response.\n  - No `scope` parameter and no scopes are defined.\n  - Either `secret` or `client_secret` is accepted for the same value.\n  failure_modes:\n  - {status: 403, meaning: 'Invalid credentials — note this is 403, not the usual 401'}\n  - {status: 422, meaning: 'Invalid parameters (e.g. missing client_id)'}\n  observed:\n  - {url: 'https://api.frayt.com/api/v2.2/oauth/token', method: POST, body: 'dummy client_id/secret', status: 403}\ncredential_issuance:\n  self_service: false\n  process: >-\n    FRAYT issues a client_id and secret manually on request. There is no developer\n\
  \    signup form and no key-management console documented.\n  contacts:\n  - {email: 'dev@frayt.com', source: 'OpenAPI info.description'}\n  - {email: 'api@frayt.com', source: 'https://www.frayt.com/frayt-api'}\n  - {email: 'integrations@frayt.com', source: 'https://www.frayt.com/3pl/api'}\n  environments_note: >-\n    Credentials are environment-bound. Sandbox and production are separated by\n    hostname, not by a key prefix. See sandbox/frayt-sandbox.yml.\ntoken_lifetime:\n  documented: false\n  note: >-\n    Neither the spec nor the docs state how long a bearer token is valid, and the\n    token response carries no expiry. Clients must detect expiry reactively by\n    handling a 403 and re-issuing.\ndiscovery:\n  openid_configuration: {status: 404}\n  oauth_authorization_server: {status: 404}\n  oauth_protected_resource: {status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frayt/refs/heads/main/authentication/frayt-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Last Mile Delivery
- Logistics
- Couriers
- On-Demand Delivery
- Shipping
- Freight
- Supply Chain
- Transportation
- Third Party Logistics
- Delivery Tracking
- Webhook
---
