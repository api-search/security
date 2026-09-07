---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chaoss-collectoss-openapi.yml
  format: yaml
  label: CollectOSS REST API
  slug: collectoss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-collectoss-openapi.yml
auth_types: []
description: 'CollectOSS implements OAuth 2.0 authorization code grant, and each CollectOSS deployment acts as its own authorization server. There is no CHAOSS-operated identity provider: credentials are issued by whichever instance you are calling. Authenticated requests carry BOTH the client secret and the user bearer token in a single Authorization header, which is a non-standard composition and is the single most important thing an integrator or agent has to get right.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chaoss Authentication
name_suffix: Authentication
oauth_flows: []
overview: CHAOSS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CHAOSS
provider_slug: chaoss
scheme_count: 2
schemes:
- authorization_endpoint: /user/authorize
  authorization_params:
  - description: The Application ID issued when the Client Application was registered.
    name: client_id
    required: true
  - name: response_type
    required: true
    value: code
  - description: Optional caller-defined value echoed back on redirect.
    name: state
    required: false
  description: Three-legged OAuth 2.0. The flow must be initiated by explicit user intent — the docs state the application "must not request initial authorization on the user's behalf, and must not automatically redirect the user to the authorization server."
  flow: authorizationCode
  header: Authorization
  id: oauth2_authorization_code
  in: header
  refresh_endpoint: /api/unstable/user/session/refresh
  refresh_operation_id: Refresh User Session Token
  refresh_params:
  - in: query
    name: refresh_token
    required: true
  - in: query
    name: grant_type
    required: true
    value: refresh_token
  - format: Client [client secret]
    in: header
    name: Authorization
    required: true
  refresh_rotation: Both the access token and the refresh token may be rotated. The docs state the returned bearer token may or may not equal the current one, and that when it differs, the previous bearer token AND the previous refresh token are invalidated. A refresh token may only be used by the application that issued it — reuse by another application returns status "Invalid application".
  scopes: []
  scopes_note: No OAuth scopes are defined. The authorization page is documented as telling the user "what information will be shared", but neither the docs nor the contract enumerate a scope vocabulary, so authorization is all-or-nothing per application.
  token_endpoint: /api/unstable/user/session/generate
  token_lifetime: Variable. The token response carries an `expires` integer (seconds until the access_token expires); no fixed default is published.
  token_operation_id: Generate User Session Token
  token_params:
  - description: The temporary authorization code, one-time use and valid for seconds only.
    in: query
    name: code
    required: true
  - in: query
    name: grant_type
    required: true
    value: code
  - format: Client [client secret]
    in: header
    name: Authorization
    required: true
  token_response_fields:
  - status
  - username
  - access_token
  - refresh_token
  - token_type
  - expires
  type: oauth2
- applies_to_operations:
  - DEI Badging Tracking
  - DEI Badging Report
  - Generate User Session Token
  - Refresh User Session Token
  description: The client secret alone authenticates the two DEI Badging write operations (POST /dei/repo/add, POST /dei/report) and the two token endpoints. Each declares the Authorization header as required with description "Client [API_Key]".
  format: Client [client secret]
  header: Authorization
  id: client_credential_header
  in: header
  type: apiKey
slug: chaoss-authentication
source_filename: chaoss-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: CHAOSS\nproviderId: chaoss\napi: CollectOSS REST API\ngenerated: '2026-09-05'\nmodified: '2026-09-05'\nmethod: searched\nsource: >-\n  https://docs.collectoss.org/en/latest/login.html (\"CollectOSS OAuth Flow\", HTTP 200, fetched\n  2026-09-05) reconciled against the login operations in the published contract\n  openapi/chaoss-collectoss-openapi.yml (POST /user/session/generate, POST /user/session/refresh).\ndocs: https://docs.collectoss.org/en/latest/login.html\ndescription: >-\n  CollectOSS implements OAuth 2.0 authorization code grant, and each CollectOSS deployment acts as\n  its own authorization server. There is no CHAOSS-operated identity provider: credentials are issued\n  by whichever instance you are calling. Authenticated requests carry BOTH the client secret and the\n  user bearer token in a single Authorization header, which is a non-standard composition and is the\n  single most\
  \ important thing an integrator or agent has to get right.\nspec_gap: >-\n  The published OpenAPI declares NO components.securitySchemes and no top-level security block. The\n  auth model below is read entirely from the prose documentation and from the header parameters on\n  the four POST operations, each of which declares `Authorization: Client [API_Key]` as a required\n  header. An agent consuming only the machine-readable contract would conclude the API is anonymous.\nschemes:\n  - id: oauth2_authorization_code\n    type: oauth2\n    flow: authorizationCode\n    in: header\n    header: Authorization\n    description: >-\n      Three-legged OAuth 2.0. The flow must be initiated by explicit user intent — the docs state the\n      application \"must not request initial authorization on the user's behalf, and must not\n      automatically redirect the user to the authorization server.\"\n    authorization_endpoint: /user/authorize\n    authorization_params:\n      - name: client_id\n \
  \       required: true\n        description: The Application ID issued when the Client Application was registered.\n      - name: response_type\n        required: true\n        value: code\n      - name: state\n        required: false\n        description: Optional caller-defined value echoed back on redirect.\n    token_endpoint: /api/unstable/user/session/generate\n    token_operation_id: Generate User Session Token\n    token_params:\n      - name: code\n        in: query\n        required: true\n        description: The temporary authorization code, one-time use and valid for seconds only.\n      - name: grant_type\n        in: query\n        required: true\n        value: code\n      - name: Authorization\n        in: header\n        required: true\n        format: 'Client [client secret]'\n    token_response_fields: [status, username, access_token, refresh_token, token_type, expires]\n    refresh_endpoint: /api/unstable/user/session/refresh\n    refresh_operation_id: Refresh User\
  \ Session Token\n    refresh_params:\n      - name: refresh_token\n        in: query\n        required: true\n      - name: grant_type\n        in: query\n        required: true\n        value: refresh_token\n      - name: Authorization\n        in: header\n        required: true\n        format: 'Client [client secret]'\n    refresh_rotation: >-\n      Both the access token and the refresh token may be rotated. The docs state the returned bearer\n      token may or may not equal the current one, and that when it differs, the previous bearer token\n      AND the previous refresh token are invalidated. A refresh token may only be used by the\n      application that issued it — reuse by another application returns status \"Invalid application\".\n    token_lifetime: >-\n      Variable. The token response carries an `expires` integer (seconds until the access_token\n      expires); no fixed default is published.\n    scopes: []\n    scopes_note: >-\n      No OAuth scopes are defined. The\
  \ authorization page is documented as telling the user \"what\n      information will be shared\", but neither the docs nor the contract enumerate a scope\n      vocabulary, so authorization is all-or-nothing per application.\n  - id: client_credential_header\n    type: apiKey\n    in: header\n    header: Authorization\n    format: 'Client [client secret]'\n    description: >-\n      The client secret alone authenticates the two DEI Badging write operations\n      (POST /dei/repo/add, POST /dei/report) and the two token endpoints. Each declares the\n      Authorization header as required with description \"Client [API_Key]\".\n    applies_to_operations:\n      - DEI Badging Tracking\n      - DEI Badging Report\n      - Generate User Session Token\n      - Refresh User Session Token\nauthenticated_request_format:\n  header: Authorization\n  value: 'Client [Client Secret], Bearer [User Session Token]'\n  note: >-\n    Both credentials must be present in the SAME Authorization header, comma-separated.\
  \ This is not\n    RFC 7235 credential syntax and will break naive clients and most generated SDKs, which assume a\n    single scheme token per header.\nregistration:\n  self_service: true\n  steps:\n    - Register a user account on the target CollectOSS instance via Login -> Register.\n    - Open your username -> Profile -> Applications.\n    - Create an application with a name and a redirect URL reachable by the user's browser.\n    - Record the Application ID and Client Secret shown after creation.\n  local_testing_note: >-\n    The docs explicitly allow http://127.0.0.1/ or http://localho.st as a redirect host for local\n    testing, and warn that the authorization server does not verify the redirect URL is reachable.\ndeployment_prerequisite: >-\n  Instances behind Nginx or Apache must set `proxy_set_header X-Forwarded-Proto $scheme;` (or the\n  Apache equivalent) or the OAuth flow will not work.\nunauthenticated_surface: >-\n  The 133 GET metric operations declare no Authorization\
  \ header in the contract. Whether they are\n  in fact anonymous is an instance deployment decision and is not stated in the documentation;\n  this artifact does not assert that they are.\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/authentication/chaoss-authentication.yml
summary_line: 2 schemes
tags:
- Analytics
- Community Health
- DEI
- Linux Foundation
- Metrics
- Observability
- Open-Source
- Risk
- Sustainability
---
