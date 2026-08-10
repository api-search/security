---
api_key_in:
- header
api_specs:
- filename: climateai-platform-swagger.json
  format: json
  label: ClimateAI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/_original/climateai-platform-swagger.json
- filename: climateai-account-api-openapi.yml
  format: yaml
  label: ClimateAI Account API
  slug: climateai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-account-api-openapi.yml
- filename: climateai-account-config-api-openapi.yml
  format: yaml
  label: ClimateAI Account Config API
  slug: climateai-account-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-account-config-api-openapi.yml
- filename: climateai-auth-api-openapi.yml
  format: yaml
  label: ClimateAI Auth API
  slug: climateai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-auth-api-openapi.yml
- filename: climateai-current-v2-api-openapi.yml
  format: yaml
  label: ClimateAI Current (v2) API
  slug: climateai-current-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-current-v2-api-openapi.yml
- filename: climateai-device-api-openapi.yml
  format: yaml
  label: ClimateAI Device API
  slug: climateai-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-device-api-openapi.yml
- filename: climateai-email-api-openapi.yml
  format: yaml
  label: ClimateAI Email API
  slug: climateai-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-email-api-openapi.yml
- filename: climateai-legacy-v1-api-openapi.yml
  format: yaml
  label: ClimateAI Legacy (v1) API
  slug: climateai-legacy-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-legacy-v1-api-openapi.yml
- filename: climateai-permission-api-openapi.yml
  format: yaml
  label: ClimateAI Permission API
  slug: climateai-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-permission-api-openapi.yml
- filename: climateai-platform-api-openapi.yml
  format: yaml
  label: ClimateAI Platform API
  slug: climateai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-platform-api-openapi.yml
- filename: climateai-product-api-openapi.yml
  format: yaml
  label: ClimateAI Product API
  slug: climateai-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-product-api-openapi.yml
- filename: climateai-report-api-openapi.yml
  format: yaml
  label: ClimateAI Report API
  slug: climateai-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-report-api-openapi.yml
- filename: climateai-role-api-openapi.yml
  format: yaml
  label: ClimateAI Role API
  slug: climateai-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-role-api-openapi.yml
- filename: climateai-routing-api-openapi.yml
  format: yaml
  label: ClimateAI Routing API
  slug: climateai-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-routing-api-openapi.yml
- filename: climateai-user-api-openapi.yml
  format: yaml
  label: ClimateAI User API
  slug: climateai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Climateai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClimateAI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClimateAI
provider_slug: climateai
scheme_count: 2
schemes:
- description: Primary developer credential for the LensConnect Weather API. Every request must carry the key in the X-Api-Key header. Keys are provisioned by ClimateAi (request one from sales@climate.ai); entitlements such as 1 km downscaling are bound to the key at the account level, so the same call returns different resolution depending on how the key is provisioned.
  docs: https://docs.climate.ai/guide/getting-started
  in: header
  name: apikey
  parameter: X-Api-Key
  provisioning: sales@climate.ai / ClimateAi account manager
  self_service: false
  sources:
  - openapi/climateai-weather-openapi.yml
  - openapi/climateai-platform-swagger.json
  type: apiKey
- description: Bearer/JWT credential used by the ClimateAI Platform gateway (default security for the platform contract). Obtained through the platform auth operations; used for account, user, role, permission and routing operations rather than weather data.
  in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/climateai-platform-swagger.json
  type: apiKey
slug: climateai-authentication
source_filename: climateai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/climateai-platform-swagger.json, openapi/climateai-weather-openapi.yml\ndocs: https://docs.climate.ai/guide/getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    Key-auth only. There is no OAuth 2.0 / OpenID Connect surface on either published\n    contract, so there is no scope model to capture (scopes/ is intentionally absent).\n    Keys are issued by ClimateAi sales/account management rather than self-service.\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: >-\n    Primary developer credential for the LensConnect Weather API. Every request must\n    carry the key in the X-Api-Key header. Keys are provisioned by ClimateAi (request\n    one from sales@climate.ai); entitlements such as 1 km downscaling are bound to the\n    key at the account level, so the same call returns different resolution depending\n    on\
  \ how the key is provisioned.\n  provisioning: sales@climate.ai / ClimateAi account manager\n  self_service: false\n  docs: https://docs.climate.ai/guide/getting-started\n  sources:\n  - openapi/climateai-weather-openapi.yml\n  - openapi/climateai-platform-swagger.json\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Bearer/JWT credential used by the ClimateAI Platform gateway (default security for\n    the platform contract). Obtained through the platform auth operations; used for\n    account, user, role, permission and routing operations rather than weather data.\n  sources:\n  - openapi/climateai-platform-swagger.json\nexample: |\n  curl -X GET \"https://api-prod.climate.ai/weather/v2/history\" \\\n    -G -d \"lat=37.7\" -d \"lon=-122.4\" -d \"var=temp_mean\" \\\n    -d \"start_date=2024-01-01\" -d \"end_date=2024-12-31\" \\\n    -H \"X-Api-Key: <YOUR_API_KEY>\"\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://docs.climate.ai/guide/getting-started\n\
  \    http_status: 200\n  - url: https://docs.climate.ai/climateai-weather-api/openapi.yaml\n    http_status: 200\n  - url: https://api-prod.climate.ai/swagger.json\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/authentication/climateai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Weather
- Climate
- Climate Intelligence
- Forecasting
- Agriculture
- Data
- Supply Chain
- Risk
- Sustainability
---
