---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: citedtravel-com-billing-api-openapi.yml
  format: yaml
  label: CitedTravel Billing API
  slug: citedtravel-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citedtravel-com/openapi/citedtravel-com-billing-api-openapi.yml
- filename: citedtravel-com-entry-api-openapi.yml
  format: yaml
  label: CitedTravel Entry API
  slug: citedtravel-com-entry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citedtravel-com/openapi/citedtravel-com-entry-api-openapi.yml
- filename: citedtravel-com-facts-api-openapi.yml
  format: yaml
  label: CitedTravel Facts API
  slug: citedtravel-com-facts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citedtravel-com/openapi/citedtravel-com-facts-api-openapi.yml
- filename: citedtravel-com-meta-api-openapi.yml
  format: yaml
  label: CitedTravel Meta API
  slug: citedtravel-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citedtravel-com/openapi/citedtravel-com-meta-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Citedtravel Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CitedTravel secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CitedTravel
provider_slug: citedtravel-com
scheme_count: 3
schemes:
- description: 'API key: ct_live_… / ct_test_…'
  name: bearer
  scheme: bearer
  sources:
  - openapi/citedtravel-com-openapi.json
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/citedtravel-com-openapi.json
  type: apiKey
- description: x402 v2 payment payload (base64 JSON). See the PAYMENT-REQUIRED header of a 402 response.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/citedtravel-com-openapi.json
  type: apiKey
slug: citedtravel-com-authentication
source_filename: citedtravel-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/citedtravel-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'API key: ct_live_… / ct_test_…'\n  sources:\n  - openapi/citedtravel-com-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/citedtravel-com-openapi.json\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 v2 payment payload (base64 JSON). See the PAYMENT-REQUIRED header of a 402\n    response.\n  sources:\n  - openapi/citedtravel-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/citedtravel-com/authentication/citedtravel-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Travel
- Data
- TravelFacts
- Open Data
---
