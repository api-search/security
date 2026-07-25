---
api_key_in: []
api_specs:
- filename: atandt-device-status-api-openapi.yml
  format: yaml
  label: AT&T Device Status API
  slug: atandt-device-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-device-status-api-openapi.yml
- filename: atandt-network-insights-api-openapi.yml
  format: yaml
  label: AT&T Network Insights API
  slug: atandt-network-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-network-insights-api-openapi.yml
- filename: atandt-number-verification-api-openapi.yml
  format: yaml
  label: AT&T Number Verification API
  slug: atandt-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-number-verification-api-openapi.yml
- filename: atandt-order-management-api-openapi.yml
  format: yaml
  label: AT&T Order Management API
  slug: atandt-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-order-management-api-openapi.yml
- filename: atandt-product-ordering-api-openapi.yml
  format: yaml
  label: AT&T Product Ordering API
  slug: atandt-product-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-product-ordering-api-openapi.yml
- filename: atandt-quality-on-demand-api-openapi.yml
  format: yaml
  label: AT&T Quality on Demand API
  slug: atandt-quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-quality-on-demand-api-openapi.yml
- filename: atandt-service-qualification-api-openapi.yml
  format: yaml
  label: AT&T Service Qualification API
  slug: atandt-service-qualification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-service-qualification-api-openapi.yml
- filename: atandt-sim-swap-api-openapi.yml
  format: yaml
  label: AT&T SIM Swap API
  slug: atandt-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-sim-swap-api-openapi.yml
- filename: atandt-threat-detection-api-openapi.yml
  format: yaml
  label: AT&T Threat Detection API
  slug: atandt-threat-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-threat-detection-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Atandt Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: AT&T secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: AT&T
provider_slug: atandt
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://devex-web.att.com/oauth/token
  name: oauth2
  sources:
  - openapi/atandt-enterprise-connectivity-apis.yaml
  - openapi/atandt-network-apis.yaml
  type: oauth2
slug: atandt-authentication
source_filename: atandt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atandt-enterprise-connectivity-apis.yaml, openapi/atandt-network-apis.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://devex-web.att.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/atandt-enterprise-connectivity-apis.yaml\n  - openapi/atandt-network-apis.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/authentication/atandt-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 100
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
---
