---
api_key_in:
- query
api_specs:
- filename: live-nation-entertainment-attractions-api-openapi.yml
  format: yaml
  label: live-nation-entertainment Attractions API
  slug: live-nation-entertainment-attractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-nation-entertainment/refs/heads/main/openapi/live-nation-entertainment-attractions-api-openapi.yml
- filename: live-nation-entertainment-classifications-api-openapi.yml
  format: yaml
  label: live-nation-entertainment Classifications API
  slug: live-nation-entertainment-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-nation-entertainment/refs/heads/main/openapi/live-nation-entertainment-classifications-api-openapi.yml
- filename: live-nation-entertainment-events-api-openapi.yml
  format: yaml
  label: live-nation-entertainment Events API
  slug: live-nation-entertainment-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-nation-entertainment/refs/heads/main/openapi/live-nation-entertainment-events-api-openapi.yml
- filename: live-nation-entertainment-venues-api-openapi.yml
  format: yaml
  label: live-nation-entertainment Venues API
  slug: live-nation-entertainment-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-nation-entertainment/refs/heads/main/openapi/live-nation-entertainment-venues-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Live Nation Entertainment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Live Nation Entertainment secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Live Nation Entertainment
provider_slug: live-nation-entertainment
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: apikey
  sources:
  - openapi/live-nation-entertainment-ticketmaster-discovery-api-openapi.yml
  type: apiKey
slug: live-nation-entertainment-authentication
source_filename: live-nation-entertainment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/live-nation-entertainment-ticketmaster-discovery-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/live-nation-entertainment-ticketmaster-discovery-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/live-nation-entertainment/refs/heads/main/authentication/live-nation-entertainment-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fortune 500
---
