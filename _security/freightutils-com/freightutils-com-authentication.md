---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: freightutils-com-adr-api-openapi.yml
  format: yaml
  label: FreightUtils ADR API
  slug: freightutils-com-adr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-adr-api-openapi.yml
- filename: freightutils-com-calculators-api-openapi.yml
  format: yaml
  label: FreightUtils Calculators API
  slug: freightutils-com-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-calculators-api-openapi.yml
- filename: freightutils-com-composite-api-openapi.yml
  format: yaml
  label: FreightUtils Composite API
  slug: freightutils-com-composite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-composite-api-openapi.yml
- filename: freightutils-com-consignment-api-openapi.yml
  format: yaml
  label: FreightUtils Consignment API
  slug: freightutils-com-consignment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-consignment-api-openapi.yml
- filename: freightutils-com-customs-api-openapi.yml
  format: yaml
  label: FreightUtils Customs API
  slug: freightutils-com-customs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-customs-api-openapi.yml
- filename: freightutils-com-reference-api-openapi.yml
  format: yaml
  label: FreightUtils Reference API
  slug: freightutils-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-reference-api-openapi.yml
- filename: freightutils-com-reference-data-api-openapi.yml
  format: yaml
  label: FreightUtils Reference Data API
  slug: freightutils-com-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-reference-data-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: FreightUtils Authentication
name_suffix: Authentication
oauth_flows: []
overview: FreightUtils secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FreightUtils
provider_slug: freightutils-com
scheme_count: 2
schemes:
- description: 'Free or Pro API key (fu_…). Optional: without one a call is anonymous (25/day per address).'
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/freightutils-com-openapi.json
  type: apiKey
- description: 'The same key as Authorization: Bearer fu_…'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/freightutils-com-openapi.json
  type: http
slug: freightutils-com-authentication
source_filename: freightutils-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/freightutils-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Free or Pro API key (fu_…). Optional: without one a call is anonymous (25/day\n    per address).'\n  sources:\n  - openapi/freightutils-com-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'The same key as Authorization: Bearer fu_…'\n  sources:\n  - openapi/freightutils-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/freightutils-com/authentication/freightutils-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Logistics
- Freight
- Data
---
