---
api_key_in:
- header
api_specs:
- filename: appstorespy-openapi.json
  format: json
  label: AppstoreSpy API
  slug: appstorespy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appstorespy Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppstoreSpy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AppstoreSpy
provider_slug: appstorespy
scheme_count: 1
schemes:
- applied_to_all_operations: true
  applied_to_operations: 33
  in: header
  name: APIKeyHeader
  parameter: API-KEY
  sources:
  - openapi/appstorespy-openapi.json
  - https://api.appstorespy.com/docs
  type: apiKey
slug: appstorespy-authentication
source_filename: appstorespy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://api.appstorespy.com/docs\ndocs: https://api.appstorespy.com/docs\nderived_from: openapi/appstorespy-openapi.json\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  http_auth: false\nschemes:\n  - name: APIKeyHeader\n    type: apiKey\n    in: header\n    parameter: API-KEY\n    applied_to_operations: 33\n    applied_to_all_operations: true\n    sources:\n      - openapi/appstorespy-openapi.json\n      - https://api.appstorespy.com/docs\nkey_management:\n  issuance_url: https://appstorespy.com/account\n  documented_quote: >-\n    \"If you do not have an API Key token, you can get it on your account page\n    https://appstorespy.com/account. An API Key is required to be sent as part of\n    every request in request header.\"\n  example_request: |\n    -H 'accept: application/json'\n    -H 'API-KEY: <your_token>'\n  rotation_documented: false\n\
  \  expiry_documented: false\n  scoping: none\n  multiple_keys: not documented\n  test_vs_live_keys: false\n  key_prefix: not documented\ngating:\n  plan_required: Business ($199/month)\n  note: >-\n    The API landing page states the API \"is only available on Business plan\",\n    so an API key is obtainable only by a paying subscriber - there is no free\n    or trial API tier that can be self-served.\nfailure_modes:\n  - status: 401\n    body: '{\"message\":\"Not authenticated\",\"code\":401}'\n    trigger: API-KEY header absent\n    observed: '2026-08-22 live probe of /v1/play/info/countries'\n    declared_in_spec: false\n  - status: 403\n    body: '{\"detail\":\"...\"}'\n    trigger: Access token is not valid\n    declared_in_spec: true\n    declared_on_operations: 1\ntransport_security:\n  https_required: true\n  tls_version: TLSv1.3\n  hsts: false\n  cross_ref: security/appstorespy-domain-security.yml\nscopes:\n  applicable: false\n  note: >-\n    Key-auth only - there is no OAuth\
  \ or permission surface, so no scopes/\n    artifact is emitted rather than an empty one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/authentication/appstorespy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- mobile-apps
- app-store-optimization
- market-intelligence
- app-analytics
- google-play
- apple-app-store
- reviews-and-ratings
- download-revenue-estimates
- marketing
---
