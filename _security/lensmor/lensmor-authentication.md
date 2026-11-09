---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lensmor-actions-api-openapi.yml
  format: yaml
  label: Lensmor Actions API
  slug: lensmor-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-actions-api-openapi.yml
- filename: lensmor-contacts-api-openapi.yml
  format: yaml
  label: Lensmor Contacts API
  slug: lensmor-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-contacts-api-openapi.yml
- filename: lensmor-credits-api-openapi.yml
  format: yaml
  label: Lensmor Credits API
  slug: lensmor-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-credits-api-openapi.yml
- filename: lensmor-events-api-openapi.yml
  format: yaml
  label: Lensmor Events API
  slug: lensmor-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-events-api-openapi.yml
- filename: lensmor-exhibitors-api-openapi.yml
  format: yaml
  label: Lensmor Exhibitors API
  slug: lensmor-exhibitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-exhibitors-api-openapi.yml
- filename: lensmor-personnel-api-openapi.yml
  format: yaml
  label: Lensmor Personnel API
  slug: lensmor-personnel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-personnel-api-openapi.yml
- filename: lensmor-profile-matching-api-openapi.yml
  format: yaml
  label: Lensmor Profile Matching API
  slug: lensmor-profile-matching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-profile-matching-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lensmor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lensmor declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lensmor
provider_slug: lensmor
scheme_count: 1
schemes:
- bearerFormat: Business sk API key
  description: 'Send the full Business API key from Settings -> API Keys, e.g., Authorization: Bearer sk_your_api_key.'
  scheme: bearer
  type: http
slug: lensmor-authentication
source_filename: lensmor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: /openapi/lensmor-openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: Business sk API key\n    description: \"Send the full Business API key from Settings -> API Keys, e.g., Authorization: Bearer sk_your_api_key.\"\n"
source_yaml_url: https://artifacts.apis.io/lensmor/authentication/lensmor-authentication.yml
summary_line: 1 scheme
tags:
- Event-Intelligence
- B2B
- Software-as-a-Service
- Lead Generation
- Trade Shows
---
