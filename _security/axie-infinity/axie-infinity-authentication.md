---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Axie Infinity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Axie Infinity secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Axie Infinity
provider_slug: axie-infinity
scheme_count: 2
schemes:
- description: Application API key issued per app from the Ronin Developer Console (Applications > your app > Information tab > KEY).
  in: header
  name: ApiKeyHeader
  parameter_name: X-API-Key
  source: https://docs.skymavis.com/api/authentication
  type: apiKey
- description: The same application API key may be appended as an `apiKey` query-string parameter instead of the header. Documented by the provider as an alternative; the header form is preferred because query strings are routinely logged by intermediaries.
  in: query
  name: ApiKeyQuery
  parameter_name: apiKey
  source: https://docs.skymavis.com/api/authentication
  type: apiKey
slug: axie-infinity-authentication
source_filename: axie-infinity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://docs.skymavis.com/api/authentication\ndocs: https://docs.skymavis.com/api/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  note: >-\n    Both Axie Infinity API products (Origins, AXP) are fronted by the Sky Mavis\n    API gateway and authenticate with a single application API key. There is no\n    OAuth2 / OIDC surface on these two products — Sky Mavis operates an OAuth2 /\n    OIDC service (Ronin Waypoint, athena.skymavis.com) but it authenticates\n    players into Ronin games, not these game-data APIs. No OpenAPI description is\n    published for either product, so this profile is transcribed from the\n    provider's published authentication reference rather than derived from\n    securitySchemes.\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  description: >-\n    Application API key issued per app from the Ronin\
  \ Developer Console\n    (Applications > your app > Information tab > KEY).\n  source: https://docs.skymavis.com/api/authentication\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter_name: apiKey\n  description: >-\n    The same application API key may be appended as an `apiKey` query-string\n    parameter instead of the header. Documented by the provider as an\n    alternative; the header form is preferred because query strings are\n    routinely logged by intermediaries.\n  source: https://docs.skymavis.com/api/authentication\nkey_issuance:\n  console: https://developers.roninchain.com/console/applications/\n  steps:\n  - Sign in to the Ronin Developer Console and select or create an application.\n  - Copy the KEY value from the application's Information tab.\n  - >-\n    Request access to the specific service (for example AXP service) under the\n    app's App Permission tab — a valid key alone does not grant access to every\n    gateway product.\n  rotation: Not documented\
  \ publicly.\nauthorization:\n  model: per-application service permissions granted in the Ronin Developer Console\n  scopes: none published\n  docs: https://docs.skymavis.com/axie/axp/overview\n  note: >-\n    AXP explicitly requires \"Permission to use the AXP service\", requested in the\n    console. A 403 from the gateway indicates the app lacks the service grant\n    rather than an invalid key.\ntransport:\n  tls_required: true\n  base_url: https://api-gateway.skymavis.com/\nx-evidence:\n- url: https://docs.skymavis.com/api/authentication\n  http_status: 200\n- url: https://docs.skymavis.com/api\n  http_status: 200\n- url: https://api-gateway.skymavis.com/origins/openapi.json\n  http_status: 401\n  note: >-\n    Gateway rejects unauthenticated requests to any /origins/* path with\n    {\"message\":\"No API key found in request\"} — confirms the X-API-Key\n    requirement at the edge.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axie-infinity/refs/heads/main/authentication/axie-infinity-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Gaming
- Blockchain
- Web3
- NFT
- Game Data
- Leaderboards
- Ronin
- Play to Earn
---
