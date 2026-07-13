---
api_key_in:
- header
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Mews Connector API
  slug: mews-connector-api
  spec_type: OpenAPI
  url: https://api.mews.com/Swagger/connector/swagger.yaml
- filename: swagger.yaml
  format: yaml
  label: Mews Booking Engine API
  slug: mews-booking-engine-api
  spec_type: OpenAPI
  url: https://api.mews.com/Swagger/distributor/swagger.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mews Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mews secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mews
provider_slug: mews-systems
scheme_count: 2
schemes:
- description: Mews authentication is performed by supplying ClientToken, AccessToken and Client as fields in the JSON request body (not as HTTP headers). This securityScheme is a tooling-compatible representation of the ClientToken credential. ClientToken is unique to your application and identifies the API client.
  in: header
  name: MewsClientToken
  parameter: ClientToken
  sources:
  - openapi/mews-booking-engine-api-openapi.yml
  - openapi/mews-connector-api-billing-openapi.yml
  - openapi/mews-connector-api-configuration-openapi.yml
  - openapi/mews-connector-api-customers-openapi.yml
  - openapi/mews-connector-api-operations-openapi.yml
  - openapi/mews-connector-api-payments-openapi.yml
  - openapi/mews-connector-api-pos-openapi.yml
  - openapi/mews-connector-api-reservations-openapi.yml
  - openapi/mews-connector-api-resources-openapi.yml
  - openapi/mews-connector-api-services-openapi.yml
  type: apiKey
- description: Tooling-compatible representation of the AccessToken credential, which is supplied in the JSON request body. AccessToken is unique to the connection with a property (enterprise) and identifies the property or properties whose data and services you can access. Portfolio Access Tokens enable multi-property access with a single token.
  in: header
  name: MewsAccessToken
  parameter: AccessToken
  sources:
  - openapi/mews-booking-engine-api-openapi.yml
  - openapi/mews-connector-api-billing-openapi.yml
  - openapi/mews-connector-api-configuration-openapi.yml
  - openapi/mews-connector-api-customers-openapi.yml
  - openapi/mews-connector-api-operations-openapi.yml
  - openapi/mews-connector-api-payments-openapi.yml
  - openapi/mews-connector-api-pos-openapi.yml
  - openapi/mews-connector-api-reservations-openapi.yml
  - openapi/mews-connector-api-resources-openapi.yml
  - openapi/mews-connector-api-services-openapi.yml
  type: apiKey
slug: mews-systems-authentication
source_filename: mews-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mews-booking-engine-api-openapi.yml, openapi/mews-connector-api-billing-openapi.yml,\n  openapi/mews-connector-api-configuration-openapi.yml, openapi/mews-connector-api-customers-openapi.yml,\n  openapi/mews-connector-api-operations-openapi.yml, openapi/mews-connector-api-payments-openapi.yml,\n  openapi/mews-connector-api-pos-openapi.yml, openapi/mews-connector-api-reservations-openapi.yml,\n  openapi/mews-connector-api-resources-openapi.yml, openapi/mews-connector-api-services-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: MewsClientToken\n  type: apiKey\n  in: header\n  parameter: ClientToken\n  description: Mews authentication is performed by supplying ClientToken, AccessToken and Client\n    as fields in the JSON request body (not as HTTP headers). This securityScheme is a tooling-compatible\n    representation of the ClientToken credential. ClientToken is unique to your\
  \ application\n    and identifies the API client.\n  sources:\n  - openapi/mews-booking-engine-api-openapi.yml\n  - openapi/mews-connector-api-billing-openapi.yml\n  - openapi/mews-connector-api-configuration-openapi.yml\n  - openapi/mews-connector-api-customers-openapi.yml\n  - openapi/mews-connector-api-operations-openapi.yml\n  - openapi/mews-connector-api-payments-openapi.yml\n  - openapi/mews-connector-api-pos-openapi.yml\n  - openapi/mews-connector-api-reservations-openapi.yml\n  - openapi/mews-connector-api-resources-openapi.yml\n  - openapi/mews-connector-api-services-openapi.yml\n- name: MewsAccessToken\n  type: apiKey\n  in: header\n  parameter: AccessToken\n  description: Tooling-compatible representation of the AccessToken credential, which is supplied\n    in the JSON request body. AccessToken is unique to the connection with a property (enterprise)\n    and identifies the property or properties whose data and services you can access. Portfolio\n    Access Tokens enable multi-property\
  \ access with a single token.\n  sources:\n  - openapi/mews-booking-engine-api-openapi.yml\n  - openapi/mews-connector-api-billing-openapi.yml\n  - openapi/mews-connector-api-configuration-openapi.yml\n  - openapi/mews-connector-api-customers-openapi.yml\n  - openapi/mews-connector-api-operations-openapi.yml\n  - openapi/mews-connector-api-payments-openapi.yml\n  - openapi/mews-connector-api-pos-openapi.yml\n  - openapi/mews-connector-api-reservations-openapi.yml\n  - openapi/mews-connector-api-resources-openapi.yml\n  - openapi/mews-connector-api-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mews-systems/refs/heads/main/authentication/mews-systems-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Hospitality
- Hotel
- Property Management
- PMS
- Reservations
- Bookings
- Travel
- Payments
- Point of Sale
- Channel Manager
- Booking Engine
---
