---
api_key_in:
- header
api_specs:
- filename: ryder-fleet-management-api-openapi.yml
  format: yaml
  label: Ryder Fleet Management API
  slug: fleet-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-fleet-management-api-openapi.yml
- filename: ryder-carrier-api-openapi.yml
  format: yaml
  label: Ryder Carrier API
  slug: carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-carrier-api-openapi.yml
- filename: ryder-tm-shipment-api-openapi.yml
  format: yaml
  label: Ryder TM Shipment Management API
  slug: tm-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-tm-shipment-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ryder System Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ryder System secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ryder System
provider_slug: ryder-system
scheme_count: 2
schemes:
- in: header
  name: apiKeyAuth
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/ryder-carrier-api-openapi.yml
  - openapi/ryder-fleet-management-api-openapi.yml
  - openapi/ryder-tm-shipment-api-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://login.okta.com/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/ryder-tm-shipment-api-openapi.yml
  type: oauth2
slug: ryder-system-authentication
source_filename: ryder-system-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ryder-carrier-api-openapi.yml, openapi/ryder-fleet-management-api-openapi.yml,\n  openapi/ryder-tm-shipment-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/ryder-carrier-api-openapi.yml\n  - openapi/ryder-fleet-management-api-openapi.yml\n  - openapi/ryder-tm-shipment-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.okta.com/oauth2/v1/token\n    scopes: 0\n  sources:\n  - openapi/ryder-tm-shipment-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/authentication/ryder-system-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Fleet Management
- Logistics
- Supply Chain
- Transportation
- Trucking
- Fortune 500
---
