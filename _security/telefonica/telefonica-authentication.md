---
api_key_in: []
api_specs:
- filename: telefonica-number-verification-openapi.yml
  format: yaml
  label: Telefónica Number Verification API
  slug: number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-number-verification-openapi.yml
- filename: telefonica-sim-swap-openapi.yml
  format: yaml
  label: Telefónica SIM Swap API
  slug: sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-sim-swap-openapi.yml
- filename: telefonica-kyc-match-openapi.yml
  format: yaml
  label: Telefónica Know Your Customer Match API
  slug: kyc-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-kyc-match-openapi.yml
- filename: telefonica-location-verification-openapi.yml
  format: yaml
  label: Telefónica Location Verification API
  slug: location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-location-verification-openapi.yml
- filename: telefonica-quality-on-demand-openapi.yml
  format: yaml
  label: Telefónica Quality on Demand API
  slug: quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-quality-on-demand-openapi.yml
- filename: telefonica-device-roaming-openapi.yml
  format: yaml
  label: Telefónica Device Roaming Status API
  slug: device-roaming-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-device-roaming-openapi.yml
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Telefonica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telefónica secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telefónica
provider_slug: telefonica
scheme_count: 1
schemes:
- name: openIdConnect
  openIdConnectUrl: https://opengateway.telefonica.com/.well-known/openid-configuration
  sources:
  - openapi/telefonica-device-roaming-openapi.yml
  - openapi/telefonica-kyc-match-openapi.yml
  - openapi/telefonica-location-verification-openapi.yml
  - openapi/telefonica-number-verification-openapi.yml
  - openapi/telefonica-quality-on-demand-openapi.yml
  - openapi/telefonica-sim-swap-openapi.yml
  type: openIdConnect
slug: telefonica-authentication
source_filename: telefonica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telefonica-device-roaming-openapi.yml, openapi/telefonica-kyc-match-openapi.yml,\n  openapi/telefonica-location-verification-openapi.yml, openapi/telefonica-number-verification-openapi.yml,\n  openapi/telefonica-quality-on-demand-openapi.yml, openapi/telefonica-sim-swap-openapi.yml\nsummary:\n  types:\n  - openIdConnect\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://opengateway.telefonica.com/.well-known/openid-configuration\n  sources:\n  - openapi/telefonica-device-roaming-openapi.yml\n  - openapi/telefonica-kyc-match-openapi.yml\n  - openapi/telefonica-location-verification-openapi.yml\n  - openapi/telefonica-number-verification-openapi.yml\n  - openapi/telefonica-quality-on-demand-openapi.yml\n  - openapi/telefonica-sim-swap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/authentication/telefonica-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Telecommunications
- Mobile Network
- CAMARA
- Open Gateway
- Authentication
- Fraud Prevention
- Location Services
---
