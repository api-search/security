---
api_key_in:
- header
api_specs:
- filename: expedia-group-bookings-api-openapi.yml
  format: yaml
  label: Expedia Group Bookings API
  slug: expedia-group-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-bookings-api-openapi.yml
- filename: expedia-group-content-api-openapi.yml
  format: yaml
  label: Expedia Group Content API
  slug: expedia-group-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-content-api-openapi.yml
- filename: expedia-group-deposit-api-openapi.yml
  format: yaml
  label: Expedia Group Deposit API
  slug: expedia-group-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-deposit-api-openapi.yml
- filename: expedia-group-geography-api-openapi.yml
  format: yaml
  label: Expedia Group Geography API
  slug: expedia-group-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-geography-api-openapi.yml
- filename: expedia-group-loyalty-api-openapi.yml
  format: yaml
  label: Expedia Group Loyalty API
  slug: expedia-group-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-loyalty-api-openapi.yml
- filename: expedia-group-manage-booking-api-openapi.yml
  format: yaml
  label: Expedia Group Manage Booking API
  slug: expedia-group-manage-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-manage-booking-api-openapi.yml
- filename: expedia-group-notifications-api-openapi.yml
  format: yaml
  label: Expedia Group Notifications API
  slug: expedia-group-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-notifications-api-openapi.yml
- filename: expedia-group-orderpurchasescreen-api-openapi.yml
  format: yaml
  label: Expedia Group OrderPurchaseScreen API
  slug: expedia-group-orderpurchasescreen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-orderpurchasescreen-api-openapi.yml
- filename: expedia-group-orderpurchaseupdate-api-openapi.yml
  format: yaml
  label: Expedia Group OrderPurchaseUpdate API
  slug: expedia-group-orderpurchaseupdate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-orderpurchaseupdate-api-openapi.yml
- filename: expedia-group-property-api-openapi.yml
  format: yaml
  label: Expedia Group Property API
  slug: expedia-group-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-property-api-openapi.yml
- filename: expedia-group-rate-plan-api-openapi.yml
  format: yaml
  label: Expedia Group Rate Plan API
  slug: expedia-group-rate-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-rate-plan-api-openapi.yml
- filename: expedia-group-rate-verification-thresholds-api-openapi.yml
  format: yaml
  label: Expedia Group Rate Verification Thresholds API
  slug: expedia-group-rate-verification-thresholds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-rate-verification-thresholds-api-openapi.yml
- filename: expedia-group-room-type-amenities-api-openapi.yml
  format: yaml
  label: Expedia Group Room Type Amenities API
  slug: expedia-group-room-type-amenities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-room-type-amenities-api-openapi.yml
- filename: expedia-group-room-type-api-openapi.yml
  format: yaml
  label: Expedia Group Room Type API
  slug: expedia-group-room-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-room-type-api-openapi.yml
- filename: expedia-group-shopping-api-openapi.yml
  format: yaml
  label: Expedia Group Shopping API
  slug: expedia-group-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-group-shopping-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Expedia Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Expedia Group secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Expedia Group
provider_slug: expedia-group
scheme_count: 3
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/expedia-deposit-openapi-original.yml
  - openapi/expedia-lodging-product-openapi-original.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials
  name: orderPurchaseScreenAuth
  sources:
  - openapi/expedia-fraud-protection-openapi-original.yml
  - openapi/expedia-loyalty-openapi-original.yml
  type: oauth2
- description: The custom generated authentication header. Refer to our [signature authentication](https://developers.expediagroup.com/docs/rapid/resources/reference/signature-authentication) page for full details.
  in: header
  name: rapidAuth
  parameter: Authorization
  sources:
  - openapi/expedia-rapid-openapi-original.yml
  type: apiKey
slug: expedia-group-authentication
source_filename: expedia-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/expedia-deposit-openapi-original.yml, openapi/expedia-fraud-protection-openapi-original.yml,\n  openapi/expedia-lodging-product-openapi-original.yml, openapi/expedia-loyalty-openapi-original.yml,\n  openapi/expedia-rapid-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/expedia-deposit-openapi-original.yml\n  - openapi/expedia-lodging-product-openapi-original.yml\n- name: orderPurchaseScreenAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials\n    scopes: 1\n  sources:\n  - openapi/expedia-fraud-protection-openapi-original.yml\n  - openapi/expedia-loyalty-openapi-original.yml\n- name: rapidAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n\
  \  description: The custom generated authentication header. Refer to our [signature authentication](https://developers.expediagroup.com/docs/rapid/resources/reference/signature-authentication)\n    page for full details.\n  sources:\n  - openapi/expedia-rapid-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/authentication/expedia-group-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Flights
- Hotels
- Lodging
- Travel
- Fortune 500
---
