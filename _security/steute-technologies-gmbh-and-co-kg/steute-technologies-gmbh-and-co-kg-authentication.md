---
api_key_in:
- header
api_specs:
- filename: steute-technologies-gmbh-and-co-kg-sensor-bridge-openapi-original.json
  format: json
  label: steute nexy Sensor Bridge API
  slug: steute-nexy-sensor-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/openapi/steute-technologies-gmbh-and-co-kg-sensor-bridge-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Steute Technologies Gmbh And Co Kg Authentication
name_suffix: Authentication
oauth_flows: []
overview: steute Technologies GmbH & Co. KG secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: steute Technologies GmbH & Co. KG
provider_slug: steute-technologies-gmbh-and-co-kg
scheme_count: 2
schemes:
- bearerFormat: JWT
  in: header
  name: bearer
  obtain_via: POST /api/v2/auth/login (AuthController_login)
  parameter: JWTAuthorization
  refresh_via: GET /api/v2/auth/refresh (AuthController_refresh)
  sources:
  - openapi/steute-technologies-gmbh-and-co-kg-sensor-bridge-openapi-original.json
  token_ttl_seconds: 1800
  type: apiKey
- applies_to: outbound HTTP(S) notifications from Sensor Bridge to customer endpoints
  name: notification-basic-auth
  scheme: basic
  source: https://docs.nexy.net/docs/api-and-protocols/https-notifications/
  type: http
slug: steute-technologies-gmbh-and-co-kg-authentication
source_filename: steute-technologies-gmbh-and-co-kg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/steute-technologies-gmbh-and-co-kg-sensor-bridge-openapi-original.json\ndocs: https://docs.nexy.net/docs/sensor-bridge/rest-api/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nnotes: >-\n  The nexy Sensor Bridge API v2 uses JWT authentication carried in a custom\n  JWTAuthorization header (declared as an apiKey-in-header scheme named \"bearer\"\n  in the OpenAPI). Clients POST username/password to /api/v2/auth/login\n  (AuthController_login) to obtain an accessToken (valid 30 minutes) and a\n  refreshToken; GET /api/v2/auth/refresh (AuthController_refresh) renews them.\n  The API ships with a documented factory-default API user (username \"api\",\n  password \"steute_api\") which administrators change in the Sensor Bridge web\n  UI User Settings menu. The separate HTTP(S) notification (webhook) interface\n  supports HTTP Basic Authentication toward the customer's receiving endpoint.\n\
  schemes:\n- name: bearer\n  type: apiKey\n  in: header\n  parameter: JWTAuthorization\n  bearerFormat: JWT\n  token_ttl_seconds: 1800\n  obtain_via: 'POST /api/v2/auth/login (AuthController_login)'\n  refresh_via: 'GET /api/v2/auth/refresh (AuthController_refresh)'\n  sources:\n  - openapi/steute-technologies-gmbh-and-co-kg-sensor-bridge-openapi-original.json\n- name: notification-basic-auth\n  type: http\n  scheme: basic\n  applies_to: outbound HTTP(S) notifications from Sensor Bridge to customer endpoints\n  source: https://docs.nexy.net/docs/api-and-protocols/https-notifications/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steute-technologies-gmbh-and-co-kg/refs/heads/main/authentication/steute-technologies-gmbh-and-co-kg-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Industrial
- Manufacturing
- IIoT
- Wireless
- Sensors
- Switches
- Intralogistics
- Automation
- Medical Devices
---
