---
api_key_in: []
api_specs:
- filename: united-states-postal-service-addresses-api-openapi.yml
  format: yaml
  label: United States Postal Service Addresses API
  slug: united-states-postal-service-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/openapi/united-states-postal-service-addresses-api-openapi.yml
- filename: united-states-postal-service-carrier-pickup-api-openapi.yml
  format: yaml
  label: United States Postal Service Carrier Pickup API
  slug: united-states-postal-service-carrier-pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/openapi/united-states-postal-service-carrier-pickup-api-openapi.yml
- filename: united-states-postal-service-domestic-prices-api-openapi.yml
  format: yaml
  label: United States Postal Service Domestic Prices API
  slug: united-states-postal-service-domestic-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/openapi/united-states-postal-service-domestic-prices-api-openapi.yml
- filename: united-states-postal-service-tracking-api-openapi.yml
  format: yaml
  label: United States Postal Service Tracking API
  slug: united-states-postal-service-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/openapi/united-states-postal-service-tracking-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: United States Postal Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: United States Postal Service secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: United States Postal Service
provider_slug: united-states-postal-service
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer Token obtained from the USPS OAuth API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/united-states-postal-service-addresses-openapi.yml
  - openapi/united-states-postal-service-carrier-pickup-openapi.yml
  - openapi/united-states-postal-service-domestic-prices-openapi.yml
  - openapi/united-states-postal-service-tracking-openapi.yml
  type: http
slug: united-states-postal-service-authentication
source_filename: united-states-postal-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/united-states-postal-service-addresses-openapi.yml, openapi/united-states-postal-service-carrier-pickup-openapi.yml,\n  openapi/united-states-postal-service-domestic-prices-openapi.yml, openapi/united-states-postal-service-tracking-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer Token obtained from the USPS OAuth API.\n  sources:\n  - openapi/united-states-postal-service-addresses-openapi.yml\n  - openapi/united-states-postal-service-carrier-pickup-openapi.yml\n  - openapi/united-states-postal-service-domestic-prices-openapi.yml\n  - openapi/united-states-postal-service-tracking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/authentication/united-states-postal-service-authentication.yml
summary_line: http · 1 scheme
tags:
- Government
- Postal Service
- Shipping
- Logistics
- Address Validation
- Package Tracking
---
