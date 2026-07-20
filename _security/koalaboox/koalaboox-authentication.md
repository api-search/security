---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Koalaboox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Koalaboox secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Koalaboox
provider_slug: koalaboox
scheme_count: 1
schemes:
- description: 'Three-legged OAuth 2.0. A partner application registers to receive a client id and client secret, redirects the user to the Koalaboox authorization endpoint, and exchanges the returned authorization code for a bearer access token plus a refresh token. Access tokens are sent as `Authorization: Bearer <token>` on every API call. The token response carries `access_token`, `refresh_token` and `expires_in`.'
  flows:
  - authorizationUrl: https://connect.koalaboox.com/oauth/authorize
    authorize_parameters:
    - client_id
    - redirect_uri
    - state
    - response_type
    - scope
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    tokenUrl: https://connect.koalaboox.com/oauth/token
    token_parameters:
    - grant_type
    - client_id
    - client_secret
    - redirect_uri
    - code
  name: OAuth2
  scopes: []
  scopes_note: No scope catalogue is published. The first-party reference client sends an empty `scope` parameter on the authorization request, so authorization appears to be all-or-nothing at the connected-account level rather than scope-partitioned. No scopes/ artifact is emitted for this provider.
  sources:
  - https://github.com/koalaboox/api-refarch/blob/master/app/Koalaboox/Client.php
  - https://github.com/koalaboox/api-refarch/blob/master/config/koalaboox.php
  type: oauth2
slug: koalaboox-authentication
source_filename: koalaboox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/koalaboox/api-refarch (first-party reference architecture,\n  MIT, (c) 2019 Koalaboox) + live probes of https://connect.koalaboox.com\ndocs: https://developers.cegid.be/\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  bearer_tokens: true\n  refresh_tokens: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Three-legged OAuth 2.0. A partner application registers to receive a client id\n    and client secret, redirects the user to the Koalaboox authorization endpoint,\n    and exchanges the returned authorization code for a bearer access token plus a\n    refresh token. Access tokens are sent as `Authorization: Bearer <token>` on every\n    API call. The token response carries `access_token`, `refresh_token` and `expires_in`.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.koalaboox.com/oauth/authorize\n    tokenUrl:\
  \ https://connect.koalaboox.com/oauth/token\n    grant_types:\n    - authorization_code\n    - refresh_token\n    authorize_parameters:\n    - client_id\n    - redirect_uri\n    - state\n    - response_type\n    - scope\n    token_parameters:\n    - grant_type\n    - client_id\n    - client_secret\n    - redirect_uri\n    - code\n  scopes: []\n  scopes_note: >-\n    No scope catalogue is published. The first-party reference client sends an empty\n    `scope` parameter on the authorization request, so authorization appears to be\n    all-or-nothing at the connected-account level rather than scope-partitioned. No\n    scopes/ artifact is emitted for this provider.\n  sources:\n  - https://github.com/koalaboox/api-refarch/blob/master/app/Koalaboox/Client.php\n  - https://github.com/koalaboox/api-refarch/blob/master/config/koalaboox.php\ncsrf:\n  state_parameter: required\n  evidence: >-\n    The reference architecture generates a random `state` on redirect and rejects the\n    callback with\
  \ HTTP 422 when the state is absent from the request, absent from the\n    session, or mismatched.\n  source: https://github.com/koalaboox/api-refarch/blob/master/app/Http/Middleware/AuthenticateApiCallbackRequest.php\ntoken_handling:\n  header: 'Authorization: Bearer {access_token}'\n  accept_header_required: application/json\n  accept_header_note: >-\n    The reference client forces `Accept: application/json` on every request so the\n    API returns JSON errors instead of HTML redirects.\n  expiry_field: expires_in\n  refresh: refresh_token returned with the access token\n  revocation: >-\n    A partner disconnects by discarding the stored access token, refresh token and\n    expiry; no dedicated revocation endpoint is documented.\nverification:\n  probed: '2026-07-19'\n  observations:\n  - endpoint: POST https://connect.koalaboox.com/oauth/token\n    status: 400\n    body: '{\"error\":\"unsupported_grant_type\",\"error_description\":\"The authorization\n      grant type is not supported\
  \ by the authorization server.\",\"hint\":\"Check that\n      all required parameters have been provided\",\"message\":\"The authorization grant\n      type is not supported by the authorization server.\"}'\n    note: RFC 6749 error envelope; server is a league/oauth2-server (Laravel Passport)\n      implementation.\n  - endpoint: GET https://connect.koalaboox.com/oauth/authorize\n    status: 401\n  - endpoint: GET https://connect.koalaboox.com/api/invoices\n    status: 401\n    body: '{\"message\":\"Unauthorized\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koalaboox/refs/heads/main/authentication/koalaboox-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Invoicing
- Electronic Invoicing
- Peppol
- Accounting
- Invoice Financing
- Working Capital
- Small Business
- Fintech
- Belgium
- Spain
- OAuth
---
