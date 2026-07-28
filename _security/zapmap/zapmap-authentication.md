---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: probed
name: Zapmap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zapmap secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zapmap
provider_slug: zapmap
scheme_count: 2
schemes:
- applies_to: https://api.zap-map.com/v5/
  evidence: Every unauthenticated request under /v5/ returns HTTP 401 with the JSON body {"success":false,"resources":[],"notices":[{"type":"Error","subtype":"Missing API Key"}]}. The header name X-Api-Key is read verbatim from the first-party web client bundle at https://map.zapmap.com/assets/Container-C9Tr7wxl.js, which sends it on every call to api.zap-map.com/v5.
  in: header
  name: ClientApiKey
  parameter_name: X-Api-Key
  required: true
  scope: application-level (identifies the calling Zapmap client, not the user)
  type: apiKey
  value_note: A live key value is embedded in Zapmap's public JavaScript bundle. It is a real credential belonging to Zapmap and is intentionally not copied into this catalog, and was not used to make any authenticated request.
  value_recorded: false
- evidence: 'The web client sends `Authorization: Bearer ${account.data.accessToken}` alongside X-Api-Key on user-scoped calls; the token is obtained from the /v5/authentication/login operation. Token format, lifetime, refresh mechanism and revocation are not published and were not probed.'
  header: Authorization
  issued_by: POST https://api.zap-map.com/v5/authentication/login
  name: UserAccessToken
  required_for: user-scoped operations (account data, saved routes, favourites, charging session history, chat/comment posting)
  scheme: bearer
  type: http
  value_recorded: false
slug: zapmap-authentication
source_filename: zapmap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of https://api.zap-map.com/v5/ plus the first-party\n  Zapmap web map client bundles served from https://map.zapmap.com/assets/\n  (fetched 2026-07-27).\ndocs: null\npublished_documentation: false\nnote: >-\n  Zapmap publishes NO authentication documentation. Nothing below is taken from a\n  developer portal, because none exists; every statement here is an observation of\n  the live production host or of Zapmap's own public browser client. The Zapmap\n  Spark commercial APIs (Search, Plan, Pay) have no published auth scheme at all —\n  the scheme recorded here belongs to the undocumented api.zap-map.com/v5 client\n  API that the Zapmap consumer map and apps call, which is not offered to third\n  parties. Credential VALUES observed in the public client bundle are deliberately\n  NOT recorded in this repository.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows:\
  \ []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: ClientApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-Api-Key\n  required: true\n  applies_to: https://api.zap-map.com/v5/\n  scope: application-level (identifies the calling Zapmap client, not the user)\n  evidence: >-\n    Every unauthenticated request under /v5/ returns HTTP 401 with the JSON body\n    {\"success\":false,\"resources\":[],\"notices\":[{\"type\":\"Error\",\"subtype\":\"Missing\n    API Key\"}]}. The header name X-Api-Key is read verbatim from the first-party\n    web client bundle at\n    https://map.zapmap.com/assets/Container-C9Tr7wxl.js, which sends it on every\n    call to api.zap-map.com/v5.\n  value_recorded: false\n  value_note: >-\n    A live key value is embedded in Zapmap's public JavaScript bundle. It is a\n    real credential belonging to Zapmap and is intentionally not copied into this\n    catalog, and was not used to make any authenticated request.\n- name: UserAccessToken\n\
  \  type: http\n  scheme: bearer\n  header: Authorization\n  required_for: user-scoped operations (account data, saved routes, favourites,\n    charging session history, chat/comment posting)\n  issued_by: POST https://api.zap-map.com/v5/authentication/login\n  evidence: >-\n    The web client sends `Authorization: Bearer ${account.data.accessToken}`\n    alongside X-Api-Key on user-scoped calls; the token is obtained from the\n    /v5/authentication/login operation. Token format, lifetime, refresh mechanism\n    and revocation are not published and were not probed.\n  value_recorded: false\nnon_auth_required_headers:\n- name: client-version\n  observed_values:\n  - '4.9'\n  - '7'\n  note: >-\n    Sent by the first-party client on every /v5 call. Purpose (client gating /\n    response shaping) is not documented; recorded as observed, not explained.\nspark_apis:\n  documented_scheme: none published\n  detail: >-\n    https://www.zapmap.com/for-business/products/zapmap-spark and its Search,\
  \ Plan\n    and Pay sub-pages name no API key, OAuth 2, OpenID Connect or mTLS model. Both\n    https://www.zapmap.com/.well-known/openid-configuration and\n    https://api.zap-map.com/.well-known/openid-configuration return 404, so no OIDC\n    discovery document is served anonymously. Access to Spark runs through a sales\n    contact form and a commercial agreement.\nevidence:\n- source: https://api.zap-map.com/v5/\n  status: 401\n  kind: live-probe\n  body: '{\"success\":false,\"resources\":[],\"notices\":[{\"type\":\"Error\",\"subtype\":\"Missing\n    API Key\"}]}'\n- source: https://api.zap-map.com/v5/health\n  status: 200\n  kind: live-probe\n  note: The only unauthenticated 200 found on the API host; returns\n    {\"database\":\"OK\",\"cache\":\"OK\",\"post_max_size\":\"OK\",\"upload_max_filesize\":\"OK\"}.\n- source: https://map.zapmap.com/assets/Container-C9Tr7wxl.js\n  kind: first-party-client-bundle\n  note: Zapmap's own public web map SPA; source of the header names and the\
  \ login\n    operation.\n- source: https://map.zapmap.com/assets/index-B_UH5h7L.js\n  kind: first-party-client-bundle\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zapmap/refs/heads/main/authentication/zapmap-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Energy
- United Kingdom
- EV Charging
- Electric Vehicles
- Charge Point Data
- Mobility
- Open Data
- Utilities
- Payments
- Route Planning
---
