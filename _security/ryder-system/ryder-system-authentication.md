---
api_key_in:
- header
api_specs:
- filename: ryder-system-documents-api-openapi.yml
  format: yaml
  label: Ryder System Documents API
  slug: ryder-system-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-documents-api-openapi.yml
- filename: ryder-system-fleet-api-openapi.yml
  format: yaml
  label: Ryder System Fleet API
  slug: ryder-system-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-fleet-api-openapi.yml
- filename: ryder-system-invoices-api-openapi.yml
  format: yaml
  label: Ryder System Invoices API
  slug: ryder-system-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-invoices-api-openapi.yml
- filename: ryder-system-load-events-api-openapi.yml
  format: yaml
  label: Ryder System Load Events API
  slug: ryder-system-load-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-load-events-api-openapi.yml
- filename: ryder-system-loads-api-openapi.yml
  format: yaml
  label: Ryder System Loads API
  slug: ryder-system-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-loads-api-openapi.yml
- filename: ryder-system-locations-api-openapi.yml
  format: yaml
  label: Ryder System Locations API
  slug: ryder-system-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-locations-api-openapi.yml
- filename: ryder-system-service-history-api-openapi.yml
  format: yaml
  label: Ryder System Service History API
  slug: ryder-system-service-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-service-history-api-openapi.yml
- filename: ryder-system-ship-confirmation-api-openapi.yml
  format: yaml
  label: Ryder System Ship Confirmation API
  slug: ryder-system-ship-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-ship-confirmation-api-openapi.yml
- filename: ryder-system-ship-status-api-openapi.yml
  format: yaml
  label: Ryder System Ship Status API
  slug: ryder-system-ship-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-ship-status-api-openapi.yml
- filename: ryder-system-shipments-api-openapi.yml
  format: yaml
  label: Ryder System Shipments API
  slug: ryder-system-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-shipments-api-openapi.yml
- filename: ryder-system-tracking-api-openapi.yml
  format: yaml
  label: Ryder System Tracking API
  slug: ryder-system-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-tracking-api-openapi.yml
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
