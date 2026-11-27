---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: merxprotocol-eu-company-api-openapi.yml
  format: yaml
  label: Merx Company API
  slug: merxprotocol-eu-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merxprotocol-eu/openapi/merxprotocol-eu-company-api-openapi.yml
- filename: merxprotocol-eu-discovery-api-openapi.yml
  format: yaml
  label: Merx Discovery API
  slug: merxprotocol-eu-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merxprotocol-eu/openapi/merxprotocol-eu-discovery-api-openapi.yml
- filename: merxprotocol-eu-legal-api-openapi.yml
  format: yaml
  label: Merx Legal API
  slug: merxprotocol-eu-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merxprotocol-eu/openapi/merxprotocol-eu-legal-api-openapi.yml
- filename: merxprotocol-eu-vat-api-openapi.yml
  format: yaml
  label: Merx VAT API
  slug: merxprotocol-eu-vat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merxprotocol-eu/openapi/merxprotocol-eu-vat-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Merx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Merx secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Merx
provider_slug: merxprotocol-eu
scheme_count: 1
schemes:
- description: API key for authentication
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/merxprotocol-eu-openapi.json
  type: apiKey
slug: merxprotocol-eu-authentication
source_filename: merxprotocol-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/merxprotocol-eu-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication\n  sources:\n  - openapi/merxprotocol-eu-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/merxprotocol-eu/authentication/merxprotocol-eu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Agentic Commerce
- European Services
- Directory
---
