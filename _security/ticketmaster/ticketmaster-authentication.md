---
api_key_in:
- query
api_specs:
- filename: ticketmaster-discovery-openapi.yml
  format: yaml
  label: Ticketmaster Discovery API
  slug: ticketmaster-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-discovery-openapi.yml
- filename: ticketmaster-commerce-openapi.yml
  format: yaml
  label: Ticketmaster Commerce API
  slug: ticketmaster-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/openapi/ticketmaster-commerce-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ticketmaster Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ticketmaster secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ticketmaster
provider_slug: ticketmaster
scheme_count: 1
schemes:
- in: query
  name: ApiKeyQuery
  parameter: apikey
  sources:
  - openapi/ticketmaster-commerce-openapi.yml
  type: apiKey
slug: ticketmaster-authentication
source_filename: ticketmaster-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ticketmaster-commerce-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/ticketmaster-commerce-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ticketmaster/refs/heads/main/authentication/ticketmaster-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce
- Concerts
- Entertainment
- Events
- Sports
- Tickets
- Venues
---
