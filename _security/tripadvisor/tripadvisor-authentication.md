---
api_key_in:
- query
api_specs:
- filename: tripadvisor-content-api-openapi.yml
  format: yaml
  label: Tripadvisor Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/openapi/tripadvisor-content-api-openapi.yml
- filename: tripadvisor-hotel-availability-check-api-openapi.yml
  format: yaml
  label: Tripadvisor Hotel Availability Check API
  slug: hotel-availability-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/openapi/tripadvisor-hotel-availability-check-api-openapi.yml
- filename: tripadvisor-hotel-availability-check-api-openapi.yml
  format: yaml
  label: Tripadvisor Hotel Inventory API
  slug: hotel-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/openapi/tripadvisor-hotel-availability-check-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tripadvisor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tripadvisor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tripadvisor
provider_slug: tripadvisor
scheme_count: 1
schemes:
- description: API key passed as a query parameter. Obtain your key by registering at the Tripadvisor Developer Portal.
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/tripadvisor-content-api-openapi.yml
  type: apiKey
slug: tripadvisor-authentication
source_filename: tripadvisor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tripadvisor-content-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key passed as a query parameter. Obtain your key by registering at the Tripadvisor\n    Developer Portal.\n  sources:\n  - openapi/tripadvisor-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/authentication/tripadvisor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Attractions
- Hotels
- Hospitality
- Restaurants
- Reviews
- Travel
---
