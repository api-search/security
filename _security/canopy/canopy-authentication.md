---
anonymous_access: false
api_key_in: []
api_specs:
- filename: canopy-openapi.json
  format: json
  label: Canopy Connect API
  slug: canopy-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canopy/refs/heads/main/openapi/canopy-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Canopy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canopy Connect secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Canopy Connect
provider_slug: canopy
scheme_count: 2
schemes:
- alternate_headers:
  - x-canopy-client-id
  - x-canopy-client-secret
  alternate_note: The Apps guide states that x-canopy-client-id / x-canopy-client-secret are an alternative to the Authorization header for calls against your own Team, and that sending them alongside a Bearer token causes the Authorization header to be ignored.
  applied: global (security[] on the document root)
  declared_in: openapi/canopy-openapi.json
  description: HTTP Basic authentication over HTTPS. Create the key pair in the Canopy Connect dashboard under Settings > API. The Client Secret is shown once at creation and cannot be re-retrieved; losing it requires creating a new key with a new Client ID. Canopy explicitly warns the secret is server-side only and must never be embedded in browser or mobile code.
  header: 'Authorization: Basic <base64(client_id:client_secret)>'
  name: BasicAuth
  password: Client Secret
  scheme: basic
  sources:
  - openapi/canopy-openapi.json
  - https://docs.usecanopy.com/reference/authentication-guide
  type: http
  username: Client ID
- authorization_url: https://app.usecanopy.com/oauth2/authorize
  declared_in: docs only
  description: OAuth 2.0 authorization-code flow with mandatory PKCE, used by Canopy Connect Apps to act on another Team's behalf. This flow is NOT declared in the provider's published OpenAPI - the spec carries only BasicAuth - so it is recorded here from the docs and mirrored in overlays/canopy-openapi-overlay.yaml.
  flow: authorizationCode
  name: CanopyAppsOAuth2
  pkce: required
  pkce_methods:
  - S256
  - plain
  pkce_note: S256 strongly recommended by the provider; plain accepted.
  response_modes:
  - query
  - fragment
  - form_post
  scopes_artifact: scopes/canopy-scopes.yml
  sources:
  - https://docs.usecanopy.com/reference/apps-authorization
  - https://docs.usecanopy.com/reference/apps-api-requests
  state: supported and recommended (CSRF nonce / round-trip state)
  token_header: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: canopy-authentication
source_filename: canopy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.usecanopy.com/reference/authentication-guide\ndocs:\n  - https://docs.usecanopy.com/reference/authentication-guide\n  - https://docs.usecanopy.com/reference/apps-authorization\n  - https://docs.usecanopy.com/reference/apps-api-requests\nspec: openapi/canopy-openapi.json\nsummary:\n  types:\n    - http\n    - oauth2\n  primary: HTTP Basic (Client ID as username, Client Secret as password)\n  transport: HTTPS only; TLS 1.2 and above. HTTP and TLS below 1.2 are rejected.\n  key_management: https://app.usecanopy.com/dashboard/settings/api-settings\n  environments:\n    - name: sandbox\n      note: Sandbox API keys work only against sandbox links/widgets and cannot read production data.\n    - name: production\n      note: Production API keys work only against production links and cannot read sandbox data.\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    declared_in: openapi/canopy-openapi.json\n\
  \    applied: global (security[] on the document root)\n    username: Client ID\n    password: Client Secret\n    header: 'Authorization: Basic <base64(client_id:client_secret)>'\n    description: >-\n      HTTP Basic authentication over HTTPS. Create the key pair in the Canopy\n      Connect dashboard under Settings > API. The Client Secret is shown once at\n      creation and cannot be re-retrieved; losing it requires creating a new key\n      with a new Client ID. Canopy explicitly warns the secret is server-side\n      only and must never be embedded in browser or mobile code.\n    alternate_headers:\n      - x-canopy-client-id\n      - x-canopy-client-secret\n    alternate_note: >-\n      The Apps guide states that x-canopy-client-id / x-canopy-client-secret are\n      an alternative to the Authorization header for calls against your own\n      Team, and that sending them alongside a Bearer token causes the\n      Authorization header to be ignored.\n    sources:\n      - openapi/canopy-openapi.json\n\
  \      - https://docs.usecanopy.com/reference/authentication-guide\n  - name: CanopyAppsOAuth2\n    type: oauth2\n    flow: authorizationCode\n    pkce: required\n    pkce_methods:\n      - S256\n      - plain\n    pkce_note: S256 strongly recommended by the provider; plain accepted.\n    authorization_url: https://app.usecanopy.com/oauth2/authorize\n    token_header: 'Authorization: Bearer <access_token>'\n    response_modes:\n      - query\n      - fragment\n      - form_post\n    state: supported and recommended (CSRF nonce / round-trip state)\n    scopes_artifact: scopes/canopy-scopes.yml\n    declared_in: docs only\n    description: >-\n      OAuth 2.0 authorization-code flow with mandatory PKCE, used by Canopy\n      Connect Apps to act on another Team's behalf. This flow is NOT declared in\n      the provider's published OpenAPI - the spec carries only BasicAuth - so it\n      is recorded here from the docs and mirrored in\n      overlays/canopy-openapi-overlay.yaml.\n    sources:\n\
  \      - https://docs.usecanopy.com/reference/apps-authorization\n      - https://docs.usecanopy.com/reference/apps-api-requests\nfailures:\n  - status: 401\n    code: UNAUTHORIZED\n    meaning: Missing, malformed, or invalid credentials, or an inactive key.\n  - status: 403\n    code: FORBIDDEN\n    meaning: Authenticated but not permitted for this resource.\n  - status: 403\n    code: SUBSCRIPTION_INACTIVE\n    meaning: The Team's Canopy Connect subscription is not active.\n  - status: 400\n    code: INCORRECT_API_KEY_TYPE\n    meaning: A sandbox key was used against a production link, or vice versa.\ngaps:\n  - The OpenAPI declares no oauth2 securityScheme, so scope requirements are invisible to any generated client.\n  - No /.well-known/oauth-authorization-server or /.well-known/openid-configuration is served on any host (probed 2026-09-05, 404 on usecanopy.com, www and docs).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canopy/refs/heads/main/authentication/canopy-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Auto Insurance
- Casualty
- Financial-Services
- Homeowners Insurance
- Insurance
- Insurance Verification
- Property
---
