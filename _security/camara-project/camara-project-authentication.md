---
api_key_in: []
api_specs:
- filename: number-verification-openapi.yml
  format: yaml
  label: CAMARA Number Verification API
  slug: number-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/number-verification-openapi.yml
- filename: sim-swap-openapi.yml
  format: yaml
  label: CAMARA SIM Swap API
  slug: sim-swap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/sim-swap-openapi.yml
- filename: device-location-retrieval-openapi.yml
  format: yaml
  label: CAMARA Device Location API
  slug: device-location
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/device-location-retrieval-openapi.yml
- filename: quality-on-demand-openapi.yml
  format: yaml
  label: CAMARA Quality on Demand API
  slug: quality-on-demand
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/quality-on-demand-openapi.yml
- filename: device-status-connected-network-type-openapi.yml
  format: yaml
  label: CAMARA Device Status API
  slug: device-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/device-status-connected-network-type-openapi.yml
- filename: kyc-match-openapi.yml
  format: yaml
  label: CAMARA Know Your Customer API
  slug: know-your-customer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/kyc-match-openapi.yml
- filename: one-time-password-sms-openapi.yml
  format: yaml
  label: CAMARA One Time Password SMS API
  slug: one-time-password-sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/one-time-password-sms-openapi.yml
- filename: device-swap-openapi.yml
  format: yaml
  label: CAMARA Device Swap API
  slug: device-swap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/device-swap-openapi.yml
- filename: simple-edge-discovery-openapi.yml
  format: yaml
  label: CAMARA Simple Edge Discovery API
  slug: simple-edge-discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/simple-edge-discovery-openapi.yml
- filename: carrier-billing-openapi.yml
  format: yaml
  label: CAMARA Carrier Billing Checkout API
  slug: carrier-billing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/carrier-billing-openapi.yml
- filename: population-density-data-openapi.yml
  format: yaml
  label: CAMARA Population Density Data API
  slug: population-density-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/population-density-data-openapi.yml
- filename: home-devices-qod-openapi.yml
  format: yaml
  label: CAMARA Home Devices Quality on Demand API
  slug: home-devices-qod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/home-devices-qod-openapi.yml
- filename: call-forwarding-signal-openapi.yml
  format: yaml
  label: CAMARA Call Forwarding Signal API
  slug: call-forwarding-signal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/call-forwarding-signal-openapi.yml
- filename: sms-openapi.yml
  format: yaml
  label: CAMARA Short Message Service API
  slug: sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/sms-openapi.yml
- filename: connectivity-insights-openapi.yml
  format: yaml
  label: CAMARA Connectivity Insights API
  slug: connectivity-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/connectivity-insights-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Camara Project Authentication
name_suffix: Authentication
oauth_flows: []
overview: CAMARA Project secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CAMARA Project
provider_slug: camara-project
scheme_count: 2
schemes:
- description: to support Consent Management
  name: openId
  openIdConnectUrl: https://example.com/.well-known/openid-configuration
  sources:
  - openapi/call-forwarding-signal-openapi.yml
  - openapi/carrier-billing-openapi.yml
  - openapi/connectivity-insights-openapi.yml
  - openapi/device-location-geofencing-openapi.yml
  - openapi/device-location-retrieval-openapi.yml
  - openapi/device-location-verification-openapi.yml
  - openapi/device-status-connected-network-type-openapi.yml
  - openapi/device-status-reachability-openapi.yml
  - openapi/device-status-roaming-openapi.yml
  - openapi/device-swap-openapi.yml
  - openapi/home-devices-qod-openapi.yml
  - openapi/kyc-age-verification-openapi.yml
  - openapi/kyc-fill-in-openapi.yml
  - openapi/kyc-match-openapi.yml
  - openapi/number-verification-openapi.yml
  - openapi/one-time-password-sms-openapi.yml
  - openapi/population-density-data-openapi.yml
  - openapi/qos-profiles-openapi.yml
  - openapi/qos-provisioning-openapi.yml
  - openapi/quality-on-demand-openapi.yml
  - openapi/sim-swap-openapi.yml
  - openapi/sim-swap-subscriptions-openapi.yml
  - openapi/simple-edge-discovery-openapi.yml
  - openapi/sms-openapi.yml
  type: openIdConnect
- bearerFormat: '{$request.body#/sinkCredential.credentialType}'
  name: notificationsBearerAuth
  scheme: bearer
  sources:
  - openapi/carrier-billing-openapi.yml
  - openapi/device-location-geofencing-openapi.yml
  - openapi/population-density-data-openapi.yml
  - openapi/qos-provisioning-openapi.yml
  - openapi/quality-on-demand-openapi.yml
  - openapi/sim-swap-subscriptions-openapi.yml
  type: http
slug: camara-project-authentication
source_filename: camara-project-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/call-forwarding-signal-openapi.yml, openapi/carrier-billing-openapi.yml, openapi/connectivity-insights-openapi.yml,\n  openapi/device-location-geofencing-openapi.yml, openapi/device-location-retrieval-openapi.yml,\n  openapi/device-location-verification-openapi.yml, openapi/device-status-connected-network-type-openapi.yml,\n  openapi/device-status-reachability-openapi.yml, openapi/device-status-roaming-openapi.yml,\n  openapi/device-swap-openapi.yml, openapi/home-devices-qod-openapi.yml, openapi/kyc-age-verification-openapi.yml\n  ...\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: openId\n  type: openIdConnect\n  openIdConnectUrl: https://example.com/.well-known/openid-configuration\n  description: to support Consent Management\n  sources:\n  - openapi/call-forwarding-signal-openapi.yml\n  - openapi/carrier-billing-openapi.yml\n  - openapi/connectivity-insights-openapi.yml\n  - openapi/device-location-geofencing-openapi.yml\n\
  \  - openapi/device-location-retrieval-openapi.yml\n  - openapi/device-location-verification-openapi.yml\n  - openapi/device-status-connected-network-type-openapi.yml\n  - openapi/device-status-reachability-openapi.yml\n  - openapi/device-status-roaming-openapi.yml\n  - openapi/device-swap-openapi.yml\n  - openapi/home-devices-qod-openapi.yml\n  - openapi/kyc-age-verification-openapi.yml\n  - openapi/kyc-fill-in-openapi.yml\n  - openapi/kyc-match-openapi.yml\n  - openapi/number-verification-openapi.yml\n  - openapi/one-time-password-sms-openapi.yml\n  - openapi/population-density-data-openapi.yml\n  - openapi/qos-profiles-openapi.yml\n  - openapi/qos-provisioning-openapi.yml\n  - openapi/quality-on-demand-openapi.yml\n  - openapi/sim-swap-openapi.yml\n  - openapi/sim-swap-subscriptions-openapi.yml\n  - openapi/simple-edge-discovery-openapi.yml\n  - openapi/sms-openapi.yml\n- name: notificationsBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: '{$request.body#/sinkCredential.credentialType}'\n\
  \  sources:\n  - openapi/carrier-billing-openapi.yml\n  - openapi/device-location-geofencing-openapi.yml\n  - openapi/population-density-data-openapi.yml\n  - openapi/qos-provisioning-openapi.yml\n  - openapi/quality-on-demand-openapi.yml\n  - openapi/sim-swap-subscriptions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/authentication/camara-project-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- API Standards
- CAMARA
- GSMA
- Linux Foundation
- Network APIs
- Open API
- Open Gateway
- Open Source
- Standards
- Telco
- Telco API Alliance
- Telecom
- Telecommunications
---
