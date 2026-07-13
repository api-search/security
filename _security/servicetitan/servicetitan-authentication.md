---
api_key_in:
- header
api_specs:
- filename: servicetitan-crm-api-openapi.yml
  format: yaml
  label: ServiceTitan CRM API
  slug: servicetitan-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-crm-api-openapi.yml
- filename: servicetitan-jpm-api-openapi.yml
  format: yaml
  label: ServiceTitan Job Planning & Management API
  slug: servicetitan-jpm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-jpm-api-openapi.yml
- filename: servicetitan-dispatch-api-openapi.yml
  format: yaml
  label: ServiceTitan Dispatch API
  slug: servicetitan-dispatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-dispatch-api-openapi.yml
- filename: servicetitan-accounting-api-openapi.yml
  format: yaml
  label: ServiceTitan Accounting API
  slug: servicetitan-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-accounting-api-openapi.yml
- filename: servicetitan-pricebook-api-openapi.yml
  format: yaml
  label: ServiceTitan Pricebook API
  slug: servicetitan-pricebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-pricebook-api-openapi.yml
- filename: servicetitan-inventory-api-openapi.yml
  format: yaml
  label: ServiceTitan Inventory API
  slug: servicetitan-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-inventory-api-openapi.yml
- filename: servicetitan-equipment-systems-api-openapi.yml
  format: yaml
  label: ServiceTitan Equipment Systems API
  slug: servicetitan-equipment-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-equipment-systems-api-openapi.yml
- filename: servicetitan-settings-api-openapi.yml
  format: yaml
  label: ServiceTitan Settings API
  slug: servicetitan-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/openapi/servicetitan-settings-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Servicetitan Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ServiceTitan secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ServiceTitan
provider_slug: servicetitan
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  sources:
  - openapi/servicetitan-accounting-api-openapi.yml
  - openapi/servicetitan-crm-api-openapi.yml
  - openapi/servicetitan-dispatch-api-openapi.yml
  - openapi/servicetitan-equipment-systems-api-openapi.yml
  - openapi/servicetitan-inventory-api-openapi.yml
  - openapi/servicetitan-jpm-api-openapi.yml
  - openapi/servicetitan-pricebook-api-openapi.yml
  - openapi/servicetitan-settings-api-openapi.yml
  type: oauth2
- in: header
  name: AppKey
  parameter: ST-App-Key
  sources:
  - openapi/servicetitan-accounting-api-openapi.yml
  - openapi/servicetitan-crm-api-openapi.yml
  - openapi/servicetitan-dispatch-api-openapi.yml
  - openapi/servicetitan-equipment-systems-api-openapi.yml
  - openapi/servicetitan-inventory-api-openapi.yml
  - openapi/servicetitan-jpm-api-openapi.yml
  - openapi/servicetitan-pricebook-api-openapi.yml
  - openapi/servicetitan-settings-api-openapi.yml
  type: apiKey
slug: servicetitan-authentication
source_filename: servicetitan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/servicetitan-accounting-api-openapi.yml, openapi/servicetitan-crm-api-openapi.yml,\n  openapi/servicetitan-dispatch-api-openapi.yml, openapi/servicetitan-equipment-systems-api-openapi.yml,\n  openapi/servicetitan-inventory-api-openapi.yml, openapi/servicetitan-jpm-api-openapi.yml,\n  openapi/servicetitan-pricebook-api-openapi.yml, openapi/servicetitan-settings-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.servicetitan.io/connect/token\n    scopes: 0\n  sources:\n  - openapi/servicetitan-accounting-api-openapi.yml\n  - openapi/servicetitan-crm-api-openapi.yml\n  - openapi/servicetitan-dispatch-api-openapi.yml\n  - openapi/servicetitan-equipment-systems-api-openapi.yml\n  - openapi/servicetitan-inventory-api-openapi.yml\n  - openapi/servicetitan-jpm-api-openapi.yml\n\
  \  - openapi/servicetitan-pricebook-api-openapi.yml\n  - openapi/servicetitan-settings-api-openapi.yml\n- name: AppKey\n  type: apiKey\n  in: header\n  parameter: ST-App-Key\n  sources:\n  - openapi/servicetitan-accounting-api-openapi.yml\n  - openapi/servicetitan-crm-api-openapi.yml\n  - openapi/servicetitan-dispatch-api-openapi.yml\n  - openapi/servicetitan-equipment-systems-api-openapi.yml\n  - openapi/servicetitan-inventory-api-openapi.yml\n  - openapi/servicetitan-jpm-api-openapi.yml\n  - openapi/servicetitan-pricebook-api-openapi.yml\n  - openapi/servicetitan-settings-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/authentication/servicetitan-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Field Service Management
- Trades
- HVAC
- Plumbing
- Electrical
- Construction
- CRM
- Dispatch
- Accounting
- Pricebook
- Marketing
- Memberships
- Webhooks
---
