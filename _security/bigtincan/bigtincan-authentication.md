---
api_key_in: []
api_specs:
- filename: bigtincan-hub-api-openapi.json
  format: json
  label: Bigtincan Hub API
  slug: bigtincan-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-hub-api-openapi.json
auth_types:
- oauth2
description: The Bigtincan Hub Public API is OAuth 2.0 only. The published Swagger 2.0 document at https://pubapi.bigtincan.com/api/sandbox/swagger/public-api declares NO securityDefinitions at all; the authentication model below was read from the provider's own interactive console at https://pubapi.bigtincan.com/doc/interactive/ (the token/authorize/revoke endpoints and grant types are defined inline in that page's JavaScript) and confirmed against live unauthenticated probes of the API host.
kind: authentication
layout: security
method: searched
name: Bigtincan Authentication
name_suffix: Authentication
oauth_flows:
- password
- authorizationCode
overview: Bigtincan secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and authorizationCode flow(s).
provider_name: Bigtincan
provider_slug: bigtincan
scheme_count: 2
schemes:
- credentials:
  - Client ID
  - Client Secret
  - API Key
  description: '"API Key Authentication" in Bigtincan''s own wording. POST client_id, client_secret and api_key with grant_type=password to the token endpoint; the response carries access_token and refresh_token. This is the flow used by server-to-server integrations, and it is the ONLY flow under which the As-User impersonation header is accepted.'
  flow: password
  name: oauth2_password
  scopes: []
  source: https://pubapi.bigtincan.com/doc/interactive/
  tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token
  type: oauth2
- authorizationUrl: https://pubapi.bigtincan.com/services/oauth2/authorize
  credentials:
  - Client ID
  - Client Secret
  description: '"User Authentication" in Bigtincan''s own wording — an interactive login with a Bigtincan Hub account. The As-User header is explicitly disabled for this flow by the console.'
  flow: authorizationCode
  name: oauth2_authorization_code
  scopes: []
  source: https://pubapi.bigtincan.com/doc/interactive/
  tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token
  type: oauth2
slug: bigtincan-authentication
source_filename: bigtincan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://pubapi.bigtincan.com/doc/interactive/\ndocs: https://pubapi.bigtincan.com/doc/interactive/\nspec: openapi/bigtincan-hub-api-openapi.json\nname: Bigtincan Hub Public API Authentication\ndescription: >-\n  The Bigtincan Hub Public API is OAuth 2.0 only. The published Swagger 2.0\n  document at https://pubapi.bigtincan.com/api/sandbox/swagger/public-api declares\n  NO securityDefinitions at all; the authentication model below was read from the\n  provider's own interactive console at\n  https://pubapi.bigtincan.com/doc/interactive/ (the token/authorize/revoke\n  endpoints and grant types are defined inline in that page's JavaScript) and\n  confirmed against live unauthenticated probes of the API host.\nsummary:\n  types:\n    - oauth2\n  oauth2_flows:\n    - password\n    - authorizationCode\n  bearer_header: 'Authorization: Bearer <access_token>'\n  refresh_supported: true\n  revocation_supported: true\n  impersonation_header:\
  \ As-User\nbase_url: https://pubapi.bigtincan.com\nendpoints:\n  - name: authorize\n    method: GET\n    url: https://pubapi.bigtincan.com/services/oauth2/authorize\n    description: >-\n      Interactive Bigtincan Hub user login (authorization code flow). Opened in a\n      popup by the \"User Login\" control on the interactive console.\n  - name: token\n    method: POST\n    url: https://pubapi.bigtincan.com/services/oauth2/token\n    description: >-\n      Issues access_token + refresh_token. Accepts grant_type=password (with\n      client_id, client_secret and api_key) and grant_type=refresh_token (with\n      client_id, client_secret and refresh_token).\n    probed:\n      status: 405\n      note: >-\n        A GET returns 405 with `allow: POST` and body\n        {\"message\":\"The requested resource does not support http method GET\"},\n        confirming the endpoint exists and is POST-only.\n  - name: revoke\n    method: POST\n    url: https://pubapi.bigtincan.com/services/oauth2/revoke\n\
  \    description: >-\n      Revokes a token. Takes `token` and `token_type_hint` of `access_token` or\n      `refresh_token`. The console revokes both on page unload and on idle.\nschemes:\n  - name: oauth2_password\n    type: oauth2\n    flow: password\n    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token\n    scopes: []\n    credentials:\n      - Client ID\n      - Client Secret\n      - API Key\n    description: >-\n      \"API Key Authentication\" in Bigtincan's own wording. POST client_id,\n      client_secret and api_key with grant_type=password to the token endpoint;\n      the response carries access_token and refresh_token. This is the flow used\n      by server-to-server integrations, and it is the ONLY flow under which the\n      As-User impersonation header is accepted.\n    source: https://pubapi.bigtincan.com/doc/interactive/\n  - name: oauth2_authorization_code\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://pubapi.bigtincan.com/services/oauth2/authorize\n\
  \    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token\n    scopes: []\n    credentials:\n      - Client ID\n      - Client Secret\n    description: >-\n      \"User Authentication\" in Bigtincan's own wording — an interactive login\n      with a Bigtincan Hub account. The As-User header is explicitly disabled for\n      this flow by the console.\n    source: https://pubapi.bigtincan.com/doc/interactive/\ndelegation:\n  header: As-User\n  value: USER_ID\n  description: >-\n    \"The As-User field allows applications to perform actions on behalf of users\n    within their tenant. Admin APIs do not support the As-User header. To perform\n    an action on behalf of a user you will need to pass this as a header:\n    As-User: USER_ID\" — quoted verbatim from\n    https://pubapi.bigtincan.com/doc/interactive/\n  constraints:\n    - Available only with the password (API Key) flow, not the authorization code flow.\n    - Admin-tagged operations do not honour As-User.\n  in_spec: >-\n\
  \    The Swagger document models As-User as an optional header parameter\n    ($ref #/definitions/As-User) on nearly every operation.\n  cors_allowed: true\nscopes:\n  published: false\n  note: >-\n    Bigtincan publishes no OAuth scope vocabulary. Neither the Swagger document\n    nor the interactive console names a single scope, and the console sets\n    scopeSeparator \",\" with an empty additionalQueryStringParams. Authorization\n    is therefore governed entirely by the Hub role/permission of the\n    authenticating user (or of the As-User target), not by token scope.\nfailure_mode:\n  status: 401\n  body: '{\"error\":{\"scope\":\"api\",\"code\":\"INVALID_TOKEN\",\"message\":\"Access token is invalid\"},\"trace_id\":\"\"}'\n  probed: 'GET https://pubapi.bigtincan.com/v1/user/me -> 401 (2026-08-14)'\ngaps:\n  - >-\n    The published Swagger 2.0 document declares no securityDefinitions and no\n    security requirement, so a generated client will emit unauthenticated calls\n    that\
  \ all fail with 401 INVALID_TOKEN. The schemes above are captured in\n    overlays/bigtincan-hub-api-overlay.yaml so the enhancement is recorded\n    separately from the provider's contract.\n  - >-\n    There is no /.well-known/oauth-authorization-server document (RFC 8414) on\n    any Bigtincan host — the OAuth endpoints are not machine-discoverable.\n  - >-\n    No scope vocabulary is published, so an agent cannot request least-privilege\n    access or reason about what a token is allowed to do.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/authentication/bigtincan-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Sales Enablement
- Content Management
- Training
- Coaching
- Buyer Engagement
- Analytics
- CRM Integration
- Digital Sales Rooms
---
