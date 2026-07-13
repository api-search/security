---
api_key_in: []
api_specs:
- filename: orange-business-number-verification-openapi.yml
  format: yaml
  label: Orange Business Number Verification API
  slug: orange-business-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-number-verification-openapi.yml
- filename: orange-business-sim-swap-openapi.yml
  format: yaml
  label: Orange Business SIM Swap API
  slug: orange-business-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-sim-swap-openapi.yml
- filename: orange-business-device-swap-openapi.yml
  format: yaml
  label: Orange Business Device Swap API
  slug: orange-business-device-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-swap-openapi.yml
- filename: orange-business-kyc-match-openapi.yml
  format: yaml
  label: Orange Business KYC Match API
  slug: orange-business-kyc-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-kyc-match-openapi.yml
- filename: orange-business-device-location-retrieval-openapi.yml
  format: yaml
  label: Orange Business Device Location Retrieval API
  slug: orange-business-device-location-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-location-retrieval-openapi.yml
- filename: orange-business-device-location-verification-openapi.yml
  format: yaml
  label: Orange Business Device Location Verification API
  slug: orange-business-device-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-location-verification-openapi.yml
- filename: orange-business-geofencing-openapi.yml
  format: yaml
  label: Orange Business Geofencing API
  slug: orange-business-geofencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-geofencing-openapi.yml
- filename: orange-business-device-reachability-status-openapi.yml
  format: yaml
  label: Orange Business Device Reachability Status API
  slug: orange-business-device-reachability-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-reachability-status-openapi.yml
- filename: orange-business-device-roaming-status-openapi.yml
  format: yaml
  label: Orange Business Device Roaming Status API
  slug: orange-business-device-roaming-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-roaming-status-openapi.yml
- filename: orange-business-quality-on-demand-openapi.yml
  format: yaml
  label: Orange Business Quality on Demand API
  slug: orange-business-quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-quality-on-demand-openapi.yml
- filename: orange-business-population-density-data-openapi.yml
  format: yaml
  label: Orange Business Population Density Data API
  slug: orange-business-population-density-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-population-density-data-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Orange Business Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orange Business secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orange Business
provider_slug: orange-business
scheme_count: 2
schemes:
- description: OpenID Connect authentication
  name: openId
  openIdConnectUrl: https://example.com/.well-known/openid-configuration
  sources:
  - openapi/orange-business-device-location-retrieval-openapi.yml
  - openapi/orange-business-device-location-verification-openapi.yml
  - openapi/orange-business-device-reachability-status-openapi.yml
  - openapi/orange-business-device-roaming-status-openapi.yml
  - openapi/orange-business-device-swap-openapi.yml
  - openapi/orange-business-geofencing-openapi.yml
  - openapi/orange-business-kyc-match-openapi.yml
  - openapi/orange-business-number-verification-openapi.yml
  - openapi/orange-business-population-density-data-openapi.yml
  - openapi/orange-business-quality-on-demand-openapi.yml
  - openapi/orange-business-sim-swap-openapi.yml
  type: openIdConnect
- bearerFormat: '{$request.body#/sinkCredential.credentialType}'
  name: notificationsBearerAuth
  scheme: bearer
  sources:
  - openapi/orange-business-geofencing-openapi.yml
  - openapi/orange-business-population-density-data-openapi.yml
  - openapi/orange-business-quality-on-demand-openapi.yml
  type: http
slug: orange-business-authentication
source_filename: orange-business-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orange-business-device-location-retrieval-openapi.yml, openapi/orange-business-device-location-verification-openapi.yml,\n  openapi/orange-business-device-reachability-status-openapi.yml, openapi/orange-business-device-roaming-status-openapi.yml,\n  openapi/orange-business-device-swap-openapi.yml, openapi/orange-business-geofencing-openapi.yml,\n  openapi/orange-business-kyc-match-openapi.yml, openapi/orange-business-number-verification-openapi.yml,\n  openapi/orange-business-population-density-data-openapi.yml, openapi/orange-business-quality-on-demand-openapi.yml,\n  openapi/orange-business-sim-swap-openapi.yml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: openId\n  type: openIdConnect\n  openIdConnectUrl: https://example.com/.well-known/openid-configuration\n  description: OpenID Connect authentication\n  sources:\n  - openapi/orange-business-device-location-retrieval-openapi.yml\n  - openapi/orange-business-device-location-verification-openapi.yml\n\
  \  - openapi/orange-business-device-reachability-status-openapi.yml\n  - openapi/orange-business-device-roaming-status-openapi.yml\n  - openapi/orange-business-device-swap-openapi.yml\n  - openapi/orange-business-geofencing-openapi.yml\n  - openapi/orange-business-kyc-match-openapi.yml\n  - openapi/orange-business-number-verification-openapi.yml\n  - openapi/orange-business-population-density-data-openapi.yml\n  - openapi/orange-business-quality-on-demand-openapi.yml\n  - openapi/orange-business-sim-swap-openapi.yml\n- name: notificationsBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: '{$request.body#/sinkCredential.credentialType}'\n  sources:\n  - openapi/orange-business-geofencing-openapi.yml\n  - openapi/orange-business-population-density-data-openapi.yml\n  - openapi/orange-business-quality-on-demand-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/authentication/orange-business-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- 5G
- AI
- B2B
- CAMARA
- Cloud
- Communications
- Cybersecurity
- Developer Platform
- Digital Workplace
- Enterprise
- France
- IoT
- Identity
- Mobile Money
- Network APIs
- Open Gateway
- Orange
- Payments
- SD-WAN
- SMS
- SASE
- Telco
- Voice
---
