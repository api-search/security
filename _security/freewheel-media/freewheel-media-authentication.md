---
api_key_in:
- header
api_specs:
- filename: freewheel-media-advertiser-buzz-openapi-original.json
  format: json
  label: FreeWheel Advertiser (Buzz) API
  slug: freewheel-media-advertiser-buzz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/openapi/freewheel-media-advertiser-buzz-openapi-original.json
- filename: freewheel-media-demand-audience-management-openapi-original.json
  format: json
  label: FreeWheel Demand Audience Management API
  slug: freewheel-media-demand-audience-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/openapi/freewheel-media-demand-audience-management-openapi-original.json
- filename: freewheel-media-demand-deal-sync-openapi-original.json
  format: json
  label: FreeWheel Demand Deal Sync API
  slug: freewheel-media-demand-deal-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/openapi/freewheel-media-demand-deal-sync-openapi-original.json
- filename: freewheel-media-demand-creative-management-openapi-original.json
  format: json
  label: FreeWheel Demand Creative Management API
  slug: freewheel-media-demand-creative-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/openapi/freewheel-media-demand-creative-management-openapi-original.json
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Freewheel Media Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: FreeWheel Media secures its APIs with oauth2, http, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: FreeWheel Media
provider_slug: freewheel-media
scheme_count: 4
schemes:
- applies_to:
  - FreeWheel Demand / Partner APIs
  - FreeWheel Publisher (MRM) APIs
  expires_in_seconds: 604800
  flow: password
  header: 'authorization: Bearer <access_token>'
  name: freewheel-oauth2-password
  notes:
  - Bearer tokens are case sensitive.
  - Credentials are issued by FreeWheel to partners; there is no self-service signup and no client-credentials flow is documented.
  - 'Password rotation is enforced on the account behind the token: 180 days for users with Streaming Hub + API access, 365 days for API-only users.'
  scopes: []
  source: https://api-docs.freewheel.tv/demand/docs/demand-api-authentication
  token_info_url: https://api.freewheel.tv/auth/token/info
  token_type: Bearer
  token_url: https://api.freewheel.tv/auth/token
  type: oauth2
- in: header
  name: bearer
  note: How the OAuth bearer token is declared in the Demand specs — the OpenAPI models it as an apiKey header rather than as an oauth2 scheme.
  parameter: Authorization
  sources:
  - openapi/freewheel-media-demand-creative-management-openapi-original.json
  - openapi/freewheel-media-demand-deal-sync-openapi-original.json
  type: apiKey
- name: sec0
  note: HTTP basic auth as declared in the Audience Management spec; the same endpoints also accept an Authorization header parameter.
  scheme: basic
  sources:
  - openapi/freewheel-media-demand-audience-management-openapi-original.json
  type: http
- applies_to:
  - FreeWheel Advertiser (Buzz) API
  login_operation: authenticate-post
  login_path: POST /authenticate
  name: buzz-session-cookie
  notes:
  - 'Session expiry is an environment setting and defaults to 100 hours; sending "keep_logged_in": true sets a second cookie with a 30-day expiration.'
  - HTTP Basic authentication is not enabled by default but can be turned on for custom Buzz installations.
  - The /authenticate endpoint is rate limited and returns 429 when exceeded.
  parameter: <buzz_key>_buzz_cookie
  source: https://api-docs.freewheel.tv/advertiser/docs/authentication
  type: cookie
slug: freewheel-media-authentication
source_filename: freewheel-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  Derived from the four harvested OpenAPI documents, then upgraded from\n  FreeWheel's own published authentication documentation.\ndocs:\n- https://api-docs.freewheel.tv/demand/docs/demand-api-authentication\n- https://api-docs.freewheel.tv/advertiser/docs/authentication\n- https://api-docs.freewheel.tv/advertiser/docs/users-passwords-and-the-api\nnote: >-\n  FreeWheel runs three different authentication models across its API estate and\n  they do not share credentials. The Partner/Demand APIs and the Publisher (MRM)\n  APIs use OAuth 2.0 with the resource-owner password grant against\n  https://api.freewheel.tv/auth/token; the Advertiser (Buzz/Beeswax) API uses a\n  session cookie obtained by POSTing credentials to /authenticate on the\n  per-customer Buzz host. No API-key model and no OAuth scopes are published, so\n  no scopes/ artifact is emitted.\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  api_key_in:\n\
  \  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: freewheel-oauth2-password\n  type: oauth2\n  flow: password\n  token_url: https://api.freewheel.tv/auth/token\n  token_info_url: https://api.freewheel.tv/auth/token/info\n  token_type: Bearer\n  header: 'authorization: Bearer <access_token>'\n  expires_in_seconds: 604800\n  scopes: []\n  applies_to:\n  - FreeWheel Demand / Partner APIs\n  - FreeWheel Publisher (MRM) APIs\n  source: https://api-docs.freewheel.tv/demand/docs/demand-api-authentication\n  notes:\n  - Bearer tokens are case sensitive.\n  - >-\n    Credentials are issued by FreeWheel to partners; there is no self-service\n    signup and no client-credentials flow is documented.\n  - >-\n    Password rotation is enforced on the account behind the token: 180 days for\n    users with Streaming Hub + API access, 365 days for API-only users.\n- name: bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  note: >-\n    How the OAuth bearer token is declared\
  \ in the Demand specs — the OpenAPI\n    models it as an apiKey header rather than as an oauth2 scheme.\n  sources:\n  - openapi/freewheel-media-demand-creative-management-openapi-original.json\n  - openapi/freewheel-media-demand-deal-sync-openapi-original.json\n- name: sec0\n  type: http\n  scheme: basic\n  note: >-\n    HTTP basic auth as declared in the Audience Management spec; the same\n    endpoints also accept an Authorization header parameter.\n  sources:\n  - openapi/freewheel-media-demand-audience-management-openapi-original.json\n- name: buzz-session-cookie\n  type: cookie\n  parameter: <buzz_key>_buzz_cookie\n  login_operation: authenticate-post\n  login_path: POST /authenticate\n  applies_to:\n  - FreeWheel Advertiser (Buzz) API\n  source: https://api-docs.freewheel.tv/advertiser/docs/authentication\n  notes:\n  - >-\n    Session expiry is an environment setting and defaults to 100 hours; sending\n    \"keep_logged_in\": true sets a second cookie with a 30-day expiration.\n\
  \  - >-\n    HTTP Basic authentication is not enabled by default but can be turned on for\n    custom Buzz installations.\n  - The /authenticate endpoint is rate limited and returns 429 when exceeded.\nadditional_headers:\n- name: X-Freewheel-Ad-Industry\n  required: true\n  applies_to: FreeWheel Demand Audience Management API\n  description: >-\n    Scopes audience and segment requests to an advertiser industry category\n    returned by the list-industries-1 operation.\n  source: openapi/freewheel-media-demand-audience-management-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/authentication/freewheel-media-authentication.yml
summary_line: oauth2/http/apiKey · 4 schemes
tags:
- Company
- Advertising
- AdTech
- Streaming TV
- Video Advertising
- Programmatic
- Media
- Publisher Monetization
- Comcast
---
