---
api_key_in: []
api_specs:
- filename: at-t-developer-hub-network-insights-api.yaml
  format: yaml
  label: AT&T Network Insights API
  slug: att-network-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-network-insights-api.yaml
- filename: at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml
  format: yaml
  label: AT&T Mobility Threat and Anomaly Detection API
  slug: att-mobility-threat-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml
- filename: at-t-developer-hub-sim-swap-api.yaml
  format: yaml
  label: AT&T SIM Swap API
  slug: att-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-sim-swap-api.yaml
- filename: at-t-developer-hub-device-status-api.yaml
  format: yaml
  label: AT&T Device Status API
  slug: att-device-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-device-status-api.yaml
- filename: at-t-developer-hub-quality-on-demand-api.yaml
  format: yaml
  label: AT&T Quality on Demand API
  slug: att-quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-quality-on-demand-api.yaml
- filename: at-t-developer-hub-number-verification-api.yaml
  format: yaml
  label: AT&T Number Verification API
  slug: att-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-number-verification-api.yaml
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
