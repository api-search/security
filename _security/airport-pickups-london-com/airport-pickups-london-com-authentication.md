---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: airport-pickups-london-com-amend-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Amend Booking API
  slug: airport-pickups-london-com-amend-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-amend-booking-api-openapi.yml
- filename: airport-pickups-london-com-book-api-openapi.yml
  format: yaml
  label: Airport Pickups London Book API
  slug: airport-pickups-london-com-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-book-api-openapi.yml
- filename: airport-pickups-london-com-cancel-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Cancel Booking API
  slug: airport-pickups-london-com-cancel-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-cancel-booking-api-openapi.yml
- filename: airport-pickups-london-com-lookup-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Lookup Booking API
  slug: airport-pickups-london-com-lookup-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-lookup-booking-api-openapi.yml
- filename: airport-pickups-london-com-quote-api-openapi.yml
  format: yaml
  label: Airport Pickups London Quote API
  slug: airport-pickups-london-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-quote-api-openapi.yml
- filename: airport-pickups-london-com-track-api-openapi.yml
  format: yaml
  label: Airport Pickups London Track API
  slug: airport-pickups-london-com-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-track-api-openapi.yml
- filename: airport-pickups-london-com-validate-flight-api-openapi.yml
  format: yaml
  label: Airport Pickups London Validate Flight API
  slug: airport-pickups-london-com-validate-flight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-validate-flight-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Airport Pickups London Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airport Pickups London secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airport Pickups London
provider_slug: airport-pickups-london-com
scheme_count: 1
schemes:
- description: API key for authentication. Register at https://mcp.airport-pickups-london.com/a2a/register to get one.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/airport-pickups-london-com-openapi.yml
  - openapi/mcp-openapi.json
  type: apiKey
slug: airport-pickups-london-com-authentication
source_filename: airport-pickups-london-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/airport-pickups-london-com-openapi.yml, openapi/mcp-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication. Register at https://mcp.airport-pickups-london.com/a2a/register\n    to get one.\n  sources:\n  - openapi/airport-pickups-london-com-openapi.yml\n  - openapi/mcp-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/airport-pickups-london-com/authentication/airport-pickups-london-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Airport
- Transport
- Taxi
- London
---
