---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cruise-itinerary-com-bulk-exports-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Bulk exports API
  slug: cruise-itinerary-com-bulk-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-bulk-exports-api-openapi.yml
- filename: cruise-itinerary-com-changes-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Changes API
  slug: cruise-itinerary-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-changes-api-openapi.yml
- filename: cruise-itinerary-com-cruise-itinerary-data-api-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Cruise Itinerary Data API
  slug: cruise-itinerary-com-cruise-itinerary-data-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-cruise-itinerary-data-api-api-openapi.yml
- filename: cruise-itinerary-com-price-index-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Price index API
  slug: cruise-itinerary-com-price-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-price-index-api-openapi.yml
- filename: cruise-itinerary-com-reference-data-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Reference data API
  slug: cruise-itinerary-com-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-reference-data-api-openapi.yml
- filename: cruise-itinerary-com-resolver-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Resolver API
  slug: cruise-itinerary-com-resolver-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-resolver-api-openapi.yml
- filename: cruise-itinerary-com-sailings-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Sailings API
  slug: cruise-itinerary-com-sailings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-sailings-api-openapi.yml
- filename: cruise-itinerary-com-service-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Service API
  slug: cruise-itinerary-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-service-api-openapi.yml
- filename: cruise-itinerary-com-ships-and-ports-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Ships and ports API
  slug: cruise-itinerary-com-ships-and-ports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-ships-and-ports-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Cruise Itinerary Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: cruise-itinerary-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: cruise-itinerary-com
provider_slug: cruise-itinerary-com
scheme_count: 2
schemes:
- description: 'Key from the dashboard: ci_live_ followed by 32 letters and digits.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cruise-itinerary-com-openapi.json
  type: http
- description: The same key, as a header.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/cruise-itinerary-com-openapi.json
  type: apiKey
slug: cruise-itinerary-com-authentication
source_filename: cruise-itinerary-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/cruise-itinerary-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Key from the dashboard: ci_live_ followed by 32 letters and digits.'\n  sources:\n  - openapi/cruise-itinerary-com-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: The same key, as a header.\n  sources:\n  - openapi/cruise-itinerary-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cruise-itinerary-com/authentication/cruise-itinerary-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Travel
- Data
- API
- Cruise
---
