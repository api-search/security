---
api_key_in: []
api_specs:
- filename: ev-energy-api-v2-openapi.yaml
  format: yaml
  label: ev.energy v2 API
  slug: ev-energy-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-energy/refs/heads/main/openapi/ev-energy-api-v2-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ev Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: ev.energy secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: ev.energy
provider_slug: ev-energy
scheme_count: 1
schemes:
- flows:
  - client_auth: HTTP Basic — base64(client_id:client_secret) in the Authorization header
    flow: clientCredentials
    note: Authorises as a single individual or organisation depending on configuration. All requests share one rate-limit bucket. Because the token does not represent one user, endpoints that need single-user context require the EvEnergy-User header set to the absolute URL of the user resource; they return 400 without it.
    scopes: 35
    tokenUrl: https://api.ev.energy/o/token/
  - authorizationUrl: https://api.ev.energy/o/authorize/
    authorization_code_lifetime: 1 minute
    flow: authorizationCode
    note: Acts on behalf of one end user; each user gets their own rate-limit bucket. The spec declares an empty scopes object for this flow even though the docs describe a user-facing consent screen listing requested scopes.
    pkce:
      code_challenge_method: S256
      note: Recommended for native apps and single-page apps that cannot keep a client secret.
      rfc: RFC 7636
      supported: true
    scopes: 0
    tokenUrl: https://api.ev.energy/o/token/
  name: oauth2
  sources:
  - openapi/ev-energy-api-v2-openapi.yaml
  - https://developers.ev.energy/docs/auth.md
  token_header: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: ev-energy-authentication
source_filename: ev-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developers.ev.energy/docs/auth.md\nderived_from: openapi/ev-energy-api-v2-openapi.yaml\ndocs: https://developers.ev.energy/docs/auth\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  self_service_registration: false\n  note: OAuth applications are created by ev.energy, not self-registered. You supply the app name, the\n    data types (scopes) you need and the redirect URI; ev.energy returns a client_id and client_secret,\n    and separate sandbox and production credential pairs.\nschemes:\n- name: oauth2\n  type: oauth2\n  token_header: 'Authorization: Bearer <access_token>'\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ev.energy/o/token/\n    scopes: 35\n    client_auth: HTTP Basic — base64(client_id:client_secret) in the Authorization header\n    note: Authorises as a single individual or organisation depending on configuration. All requests share\n\
  \      one rate-limit bucket. Because the token does not represent one user, endpoints that need single-user\n      context require the EvEnergy-User header set to the absolute URL of the user resource; they return\n      400 without it.\n  - flow: authorizationCode\n    authorizationUrl: https://api.ev.energy/o/authorize/\n    tokenUrl: https://api.ev.energy/o/token/\n    scopes: 0\n    pkce:\n      supported: true\n      code_challenge_method: S256\n      rfc: RFC 7636\n      note: Recommended for native apps and single-page apps that cannot keep a client secret.\n    authorization_code_lifetime: 1 minute\n    note: Acts on behalf of one end user; each user gets their own rate-limit bucket. The spec declares\n      an empty scopes object for this flow even though the docs describe a user-facing consent screen\n      listing requested scopes.\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n  - https://developers.ev.energy/docs/auth.md\ntoken:\n  type: Bearer\n  lifetime_seconds:\
  \ 36000\n  lifetime_human: 10 hours\n  refresh:\n    grant: refresh_token\n    endpoint: https://api.ev.energy/o/token\n  revocation:\n    endpoint: https://api.ev.energy/o/revoke_token\n    rfc: RFC 7009\n    note: The trailing slash on the revoke URL is required; without it the API returns 405.\ndiscovery:\n  rfc8414_metadata: false\n  openid_configuration: false\n  note: The v2 API publishes no /.well-known/oauth-authorization-server or /.well-known/openid-configuration.\n    api.ev.energy returns 403 for every unauthenticated path. Endpoints must be read from the docs or\n    the OpenAPI.\nscopes_artifact: scopes/ev-energy-scopes.yml\nadditional_headers:\n- header: EvEnergy-User\n  required: conditional\n  description: Absolute URL of the user resource. Supplies single-user context for client_credentials\n    tokens. Endpoints that require it return 400 when it is absent.\n- header: EvEnergy-Version\n  required: false\n  description: Overrides the API version pinned to the OAuth client.\
  \ Invalid values return 400. Echoed\n    on every response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ev-energy/refs/heads/main/authentication/ev-energy-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Utilities
- Sustainability
- Virtual Power Plant
- Demand Response
- Solar
- Home Energy
- Internet of Things
---
