---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dvla-gov-uk-authenticate-user-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) Authenticate User API
  slug: dvla-gov-uk-authenticate-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-authenticate-user-api-openapi.yml
- filename: dvla-gov-uk-change-api-key-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) Change API Key API
  slug: dvla-gov-uk-change-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-change-api-key-api-openapi.yml
- filename: dvla-gov-uk-change-password-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) Change Password API
  slug: dvla-gov-uk-change-password-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-change-password-api-openapi.yml
- filename: dvla-gov-uk-full-driver-enquiry-api-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) Full Driver Enquiry API
  slug: dvla-gov-uk-full-driver-enquiry-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-full-driver-enquiry-api-api-openapi.yml
- filename: dvla-gov-uk-new-password-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) New Password API
  slug: dvla-gov-uk-new-password-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-new-password-api-openapi.yml
- filename: dvla-gov-uk-print-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) Print API
  slug: dvla-gov-uk-print-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-print-api-openapi.yml
- filename: dvla-gov-uk-renewal-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) Renewal API
  slug: dvla-gov-uk-renewal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-renewal-api-openapi.yml
- filename: dvla-gov-uk-vehicle-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) Vehicle API
  slug: dvla-gov-uk-vehicle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-vehicle-api-openapi.yml
- filename: dvla-gov-uk-vehicle-keeper-api-openapi.yml
  format: yaml
  label: Driver and Vehicle Licensing Agency (DVLA) Vehicle Keeper API
  slug: dvla-gov-uk-vehicle-keeper-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvla-gov-uk/openapi/dvla-gov-uk-vehicle-keeper-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Driver and Vehicle Licensing Agency (DVLA) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Driver and Vehicle Licensing Agency (DVLA) secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Driver and Vehicle Licensing Agency (DVLA)
provider_slug: dvla-gov-uk
scheme_count: 3
schemes:
- description: Valid JWT token issued as a result of authentication against the API gateway.
  in: header
  name: jwtAuth
  parameter: Authorization
  sources:
  - openapi/dvla-gov-uk-driver-view-openapi.yml
  type: apiKey
- description: API key used to access the service.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/dvla-gov-uk-driver-view-openapi.yml
  - openapi/dvla-gov-uk-driving-licence-renewal-openapi.yml
  - openapi/dvla-gov-uk-kadoe-openapi.yml
  - openapi/dvla-gov-uk-print-request-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Valid JWT token issued as a result of authentication using the DVLA Authentication API
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/dvla-gov-uk-driving-licence-renewal-openapi.yml
  - openapi/dvla-gov-uk-kadoe-openapi.yml
  - openapi/dvla-gov-uk-print-request-openapi.yml
  type: http
slug: dvla-gov-uk-authentication
source_filename: dvla-gov-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/dvla-gov-uk-driver-view-openapi.yml, openapi/dvla-gov-uk-driving-licence-renewal-openapi.yml,\n  openapi/dvla-gov-uk-kadoe-openapi.yml, openapi/dvla-gov-uk-print-request-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: jwtAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Valid JWT token issued as a result of authentication against the API gateway.\n  sources:\n  - openapi/dvla-gov-uk-driver-view-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key used to access the service.\n  sources:\n  - openapi/dvla-gov-uk-driver-view-openapi.yml\n  - openapi/dvla-gov-uk-driving-licence-renewal-openapi.yml\n  - openapi/dvla-gov-uk-kadoe-openapi.yml\n  - openapi/dvla-gov-uk-print-request-openapi.yml\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Valid JWT token\
  \ issued as a result of authentication using the DVLA Authentication\n    API\n  sources:\n  - openapi/dvla-gov-uk-driving-licence-renewal-openapi.yml\n  - openapi/dvla-gov-uk-kadoe-openapi.yml\n  - openapi/dvla-gov-uk-print-request-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dvla-gov-uk/authentication/dvla-gov-uk-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Government
- United Kingdom
- Vehicles
- Driving Licences
- Transportation
- Public Sector
---
