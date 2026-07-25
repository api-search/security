---
api_key_in: []
api_specs:
- filename: telefonica-device-roaming-api-openapi.yml
  format: yaml
  label: Telefónica Device Roaming API
  slug: telefonica-device-roaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-device-roaming-api-openapi.yml
- filename: telefonica-kyc-match-api-openapi.yml
  format: yaml
  label: Telefónica KYC Match API
  slug: telefonica-kyc-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-kyc-match-api-openapi.yml
- filename: telefonica-location-verification-api-openapi.yml
  format: yaml
  label: Telefónica Location Verification API
  slug: telefonica-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-location-verification-api-openapi.yml
- filename: telefonica-number-verification-api-openapi.yml
  format: yaml
  label: Telefónica Number Verification API
  slug: telefonica-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-number-verification-api-openapi.yml
- filename: telefonica-qod-sessions-api-openapi.yml
  format: yaml
  label: Telefónica QoD Sessions API
  slug: telefonica-qod-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-qod-sessions-api-openapi.yml
- filename: telefonica-sim-swap-api-openapi.yml
  format: yaml
  label: Telefónica SIM Swap API
  slug: telefonica-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-sim-swap-api-openapi.yml
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
