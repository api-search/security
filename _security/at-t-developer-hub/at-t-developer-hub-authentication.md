---
api_key_in: []
api_specs:
- filename: at-t-developer-hub-device-connectivity-api-openapi.yml
  format: yaml
  label: AT&T Developer Hub Device Connectivity API
  slug: at-t-developer-hub-device-connectivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-device-connectivity-api-openapi.yml
- filename: at-t-developer-hub-device-roaming-api-openapi.yml
  format: yaml
  label: AT&T Developer Hub Device Roaming API
  slug: at-t-developer-hub-device-roaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-device-roaming-api-openapi.yml
- filename: at-t-developer-hub-network-metrics-api-openapi.yml
  format: yaml
  label: AT&T Developer Hub Network Metrics API
  slug: at-t-developer-hub-network-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-network-metrics-api-openapi.yml
- filename: at-t-developer-hub-number-verification-api-openapi.yml
  format: yaml
  label: AT&T Developer Hub Number Verification API
  slug: at-t-developer-hub-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-number-verification-api-openapi.yml
- filename: at-t-developer-hub-qod-sessions-api-openapi.yml
  format: yaml
  label: AT&T Developer Hub QoD Sessions API
  slug: at-t-developer-hub-qod-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-qod-sessions-api-openapi.yml
- filename: at-t-developer-hub-sim-swap-api-openapi.yml
  format: yaml
  label: AT&T Developer Hub SIM Swap API
  slug: at-t-developer-hub-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-sim-swap-api-openapi.yml
- filename: at-t-developer-hub-threat-detection-api-openapi.yml
  format: yaml
  label: AT&T Developer Hub Threat Detection API
  slug: at-t-developer-hub-threat-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-threat-detection-api-openapi.yml
- filename: at-t-developer-hub-threat-subscriptions-api-openapi.yml
  format: yaml
  label: AT&T Developer Hub Threat Subscriptions API
  slug: at-t-developer-hub-threat-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-threat-subscriptions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: At T Developer Hub Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: AT&T Developer Hub secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
scheme_count: 1
schemes:
- description: AT&T OAuth 2.0 for CAMARA network APIs
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  sources:
  - openapi/at-t-developer-hub-device-status-api.yaml
  - openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml
  - openapi/at-t-developer-hub-network-insights-api.yaml
  - openapi/at-t-developer-hub-number-verification-api.yaml
  - openapi/at-t-developer-hub-quality-on-demand-api.yaml
  - openapi/at-t-developer-hub-sim-swap-api.yaml
  type: oauth2
slug: at-t-developer-hub-authentication
source_filename: at-t-developer-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/at-t-developer-hub-device-status-api.yaml, openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml,\n  openapi/at-t-developer-hub-network-insights-api.yaml, openapi/at-t-developer-hub-number-verification-api.yaml,\n  openapi/at-t-developer-hub-quality-on-demand-api.yaml, openapi/at-t-developer-hub-sim-swap-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n    scopes: 0\n  description: AT&T OAuth 2.0 for CAMARA network APIs\n  sources:\n  - openapi/at-t-developer-hub-device-status-api.yaml\n  - openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml\n  - openapi/at-t-developer-hub-network-insights-api.yaml\n  - openapi/at-t-developer-hub-number-verification-api.yaml\n  - openapi/at-t-developer-hub-quality-on-demand-api.yaml\n  - openapi/at-t-developer-hub-sim-swap-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/authentication/at-t-developer-hub-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 100
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
---
