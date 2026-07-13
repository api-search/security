---
api_key_in:
- header
api_specs:
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Container Booking API
  slug: cargosmart-container-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Shipment Tracking API
  slug: cargosmart-shipment-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Vessel Schedule API
  slug: cargosmart-vessel-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Shipping Documentation API
  slug: cargosmart-shipping-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cargosmart Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CargoSmart secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CargoSmart
provider_slug: cargosmart
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/cargosmart-shipment-tracking-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://auth.cargosmart.com/oauth/token
  name: oauth2
  sources:
  - openapi/cargosmart-shipment-tracking-openapi.yml
  type: oauth2
slug: cargosmart-authentication
source_filename: cargosmart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cargosmart-shipment-tracking-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/cargosmart-shipment-tracking-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.cargosmart.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/cargosmart-shipment-tracking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/authentication/cargosmart-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Booking
- Container
- Documentation
- GSBN
- IQAX
- Logistics
- Maritime
- Ocean Freight
- Schedule
- Shipping
- Supply Chain
- Tracking
- Visibility
- Vessel
---
