---
api_key_in:
- query
api_specs:
- filename: seatgeek-events-api-openapi.yml
  format: yaml
  label: SeatGeek Events API
  slug: seatgeek-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-events-api-openapi.yml
- filename: seatgeek-performers-api-openapi.yml
  format: yaml
  label: SeatGeek Performers API
  slug: seatgeek-performers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-performers-api-openapi.yml
- filename: seatgeek-recommendations-api-openapi.yml
  format: yaml
  label: SeatGeek Recommendations API
  slug: seatgeek-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-recommendations-api-openapi.yml
- filename: seatgeek-taxonomies-api-openapi.yml
  format: yaml
  label: SeatGeek Taxonomies API
  slug: seatgeek-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-taxonomies-api-openapi.yml
- filename: seatgeek-venues-api-openapi.yml
  format: yaml
  label: SeatGeek Venues API
  slug: seatgeek-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-venues-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Seatgeek Authentication
name_suffix: Authentication
oauth_flows: []
overview: SeatGeek secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SeatGeek
provider_slug: seatgeek
scheme_count: 1
schemes:
- description: SeatGeek client ID obtained from the developer portal
  in: query
  name: clientId
  parameter: client_id
  sources:
  - openapi/seatgeek-platform-openapi.yml
  type: apiKey
slug: seatgeek-authentication
source_filename: seatgeek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seatgeek-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: clientId\n  type: apiKey\n  in: query\n  parameter: client_id\n  description: SeatGeek client ID obtained from the developer portal\n  sources:\n  - openapi/seatgeek-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/authentication/seatgeek-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Event
- Tickets
- Live Events
- Concerts
- Sports
- Venues
- Ticketing
---
