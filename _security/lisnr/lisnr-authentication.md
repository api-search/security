---
api_key_in:
- header
api_specs:
- filename: lisnr-tones-openapi-original.json
  format: json
  label: LISNR Tones Service API
  slug: tones-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-tones-openapi-original.json
- filename: lisnr-portal-openapi-derived.json
  format: json
  label: LISNR Portal API
  slug: portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-portal-openapi-derived.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lisnr Authentication
name_suffix: Authentication
oauth_flows: []
overview: LISNR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LISNR
provider_slug: lisnr
scheme_count: 1
schemes:
- description: An API Token prefixed by "JWT". Applied to the single Tones Service operation and to every authenticated Portal API operation.
  in: header
  name: jwtToken
  parameter: Authorization
  sources:
  - openapi/lisnr-tones-openapi-original.json
  - openapi/lisnr-portal-openapi-derived.json
  type: apiKey
  value_format: JWT <token>
slug: lisnr-authentication
source_filename: lisnr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://portal.lisnr.com/pages/developer-resources/api/api.html\ndocs: https://portal.lisnr.com/developer-resources/api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    LISNR uses no OAuth. Both the Tones Service API and the Portal API authenticate with a JWT presented in\n    the Authorization header behind the literal prefix \"JWT \" (not \"Bearer\"). There are two distinct token\n    classes, both minted per LISNR application in the Portal.\ntoken_classes:\n- name: API Token\n  used_by: LISNR Tones Service API\n  minted_at: https://portal.lisnr.com/apps/{app_id}/api-tokens\n  managed_by:\n  - openapi/lisnr-portal-openapi-derived.json#listApiTokens\n  - openapi/lisnr-portal-openapi-derived.json#createApiToken\n  - openapi/lisnr-portal-openapi-derived.json#deleteApiToken\n  description: >-\n    Authorizes external applications to call LISNR APIs on behalf of a specific LISNR application.\
  \ The\n    transaction type associated with a generated tone is inherited from the app the API token was created\n    under, so accounts with multiple transaction types must select the correct app before minting a token.\n  handling: >-\n    LISNR documents API tokens as being as sensitive as passwords. They must not be shared or distributed to\n    untrusted parties, and must not be used from a website or any other publicly available project.\n- name: SDK Token\n  used_by: Radius / Radius 3 / Point / legacy / SDA client SDKs\n  minted_at: https://portal.lisnr.com/apps/{app_id}/sdk-tokens\n  managed_by:\n  - openapi/lisnr-portal-openapi-derived.json#listSdkTokens\n  - openapi/lisnr-portal-openapi-derived.json#createSdkToken\n  - openapi/lisnr-portal-openapi-derived.json#deleteSdkToken\n  description: >-\n    Initializes the Radius object inside a device SDK. A receiving application must initialize with an SDK\n    token issued from the same account as the API token that created an encrypted\
  \ tone, otherwise it cannot\n    demodulate that tone.\n- name: User session JWT\n  used_by: LISNR Portal API\n  obtained_via: openapi/lisnr-portal-openapi-derived.json#login\n  description: >-\n    Username and password are exchanged at POST /v2/auth/login for a JWT that the Portal then sends on every\n    subsequent call in the Authorization header.\nschemes:\n- name: jwtToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: JWT <token>\n  description: >-\n    An API Token prefixed by \"JWT\". Applied to the single Tones Service operation and to every authenticated\n    Portal API operation.\n  sources:\n  - openapi/lisnr-tones-openapi-original.json\n  - openapi/lisnr-portal-openapi-derived.json\nfailure_modes:\n- status: 401\n  meaning: Authentication credentials not provided, or credentials are not valid.\n- status: 403\n  meaning: Forbidden — user is not authorized to access this resource with an explicit deny.\nrelated:\n- conventions/lisnr-conventions.yml\n\
  - errors/lisnr-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/authentication/lisnr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ultrasonic
- Data Over Audio
- Proximity
- Contactless Payments
- Device Pairing
- Identification
- Audio
- Internet of Things
- SDK
---
