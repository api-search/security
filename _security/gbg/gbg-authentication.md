---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gbg-as-api-openapi.yml
  format: yaml
  label: GBG As API
  slug: gbg-as-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-as-api-openapi.yml
- filename: gbg-authentication-api-openapi.yml
  format: yaml
  label: GBG Authentication API
  slug: gbg-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-authentication-api-openapi.yml
- filename: gbg-customer-apis-api-openapi.yml
  format: yaml
  label: GBG Customer APIs API
  slug: gbg-customer-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-customer-apis-api-openapi.yml
- filename: gbg-device-api-openapi.yml
  format: yaml
  label: GBG Device API
  slug: gbg-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-device-api-openapi.yml
- filename: gbg-end-user-apis-api-openapi.yml
  format: yaml
  label: GBG End User APIs API
  slug: gbg-end-user-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-end-user-apis-api-openapi.yml
- filename: gbg-health-api-openapi.yml
  format: yaml
  label: GBG Health API
  slug: gbg-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-health-api-openapi.yml
- filename: gbg-interaction-api-openapi.yml
  format: yaml
  label: GBG Interaction API
  slug: gbg-interaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-interaction-api-openapi.yml
- filename: gbg-interaction-service-api-openapi.yml
  format: yaml
  label: GBG Interaction Service API
  slug: gbg-interaction-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-interaction-service-api-openapi.yml
- filename: gbg-journey-api-openapi.yml
  format: yaml
  label: GBG Journey API
  slug: gbg-journey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-journey-api-openapi.yml
- filename: gbg-journey-execution-api-openapi.yml
  format: yaml
  label: GBG Journey execution API
  slug: gbg-journey-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-journey-execution-api-openapi.yml
- filename: gbg-sandbox-api-openapi.yml
  format: yaml
  label: GBG Sandbox API
  slug: gbg-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-sandbox-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gbg Authentication
name_suffix: Authentication
oauth_flows: []
overview: GBG secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GBG
provider_slug: gbg
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gbg-go-v1-openapi.yml
  - openapi/gbg-go-v2-openapi.yml
  type: http
slug: gbg-authentication
source_filename: gbg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/gbg-go-v1-openapi.yml, openapi/gbg-go-v2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/gbg-go-v1-openapi.yml\n  - openapi/gbg-go-v2-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gbg/authentication/gbg-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Identity Verification
- Fraud Prevention
- KYC
- Location Intelligence
- Compliance
- Digital Identity
---
