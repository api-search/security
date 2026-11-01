---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: titus-authorizations-api-openapi.yml
  format: yaml
  label: Titus Authorizations API
  slug: titus-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-authorizations-api-openapi.yml
- filename: titus-businessconnections-api-openapi.yml
  format: yaml
  label: Titus Business Connections API
  slug: titus-businessconnections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-businessconnections-api-openapi.yml
- filename: titus-checkouts-api-openapi.yml
  format: yaml
  label: Titus Checkouts API
  slug: titus-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-checkouts-api-openapi.yml
- filename: titus-customers-api-openapi.yml
  format: yaml
  label: Titus Customers API
  slug: titus-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-customers-api-openapi.yml
- filename: titus-listings-api-openapi.yml
  format: yaml
  label: Titus Listings API
  slug: titus-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-listings-api-openapi.yml
- filename: titus-platformpayouts-api-openapi.yml
  format: yaml
  label: Titus Platform Payouts API
  slug: titus-platformpayouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-platformpayouts-api-openapi.yml
- filename: titus-refunds-api-openapi.yml
  format: yaml
  label: Titus Refunds API
  slug: titus-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-refunds-api-openapi.yml
- filename: titus-titus-api-api-openapi.yml
  format: yaml
  label: Titus Titus API
  slug: titus-titus-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-titus-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Titus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Titus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Titus
provider_slug: titus
scheme_count: 1
schemes:
- description: API key for authentication
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/titus-original.json
  type: apiKey
slug: titus-authentication
source_filename: titus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/titus-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication\n  sources:\n  - openapi/titus-original.json\n"
source_yaml_url: https://artifacts.apis.io/titus/authentication/titus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- FinTech
- Orchestration
- API
- B2B
---
