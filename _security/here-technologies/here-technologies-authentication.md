---
api_key_in:
- query
api_specs:
- filename: here-technologies-batch-jobs-api-openapi.yml
  format: yaml
  label: HERE Technologies Batch Jobs API
  slug: here-technologies-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here-technologies/refs/heads/main/openapi/here-technologies-batch-jobs-api-openapi.yml
- filename: here-technologies-geocode-api-openapi.yml
  format: yaml
  label: HERE Technologies Geocode API
  slug: here-technologies-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here-technologies/refs/heads/main/openapi/here-technologies-geocode-api-openapi.yml
- filename: here-technologies-health-api-openapi.yml
  format: yaml
  label: HERE Technologies Health API
  slug: here-technologies-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here-technologies/refs/heads/main/openapi/here-technologies-health-api-openapi.yml
- filename: here-technologies-notifications-api-openapi.yml
  format: yaml
  label: HERE Technologies Notifications API
  slug: here-technologies-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here-technologies/refs/heads/main/openapi/here-technologies-notifications-api-openapi.yml
- filename: here-technologies-reverse-geocode-api-openapi.yml
  format: yaml
  label: HERE Technologies Reverse Geocode API
  slug: here-technologies-reverse-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here-technologies/refs/heads/main/openapi/here-technologies-reverse-geocode-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Here Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: HERE Technologies secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HERE Technologies
provider_slug: here-technologies
scheme_count: 2
schemes:
- in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/here-technologies-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/here-technologies-openapi.yml
  type: http
slug: here-technologies-authentication
source_filename: here-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/here-technologies-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/here-technologies-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/here-technologies-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/here-technologies/refs/heads/main/authentication/here-technologies-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Maps
- Geocoding
- Routing
- Location Services
- Traffic
- HD Live Map
- Automotive
- Fleet
---
