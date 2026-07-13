---
api_key_in:
- header
api_specs:
- filename: placekey-openapi.yml
  format: yaml
  label: Placekey Lookup API
  slug: placekey-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placekey/refs/heads/main/openapi/placekey-openapi.yml
- filename: placekey-openapi.yml
  format: yaml
  label: Placekey Bulk Lookup API
  slug: placekey-bulk-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placekey/refs/heads/main/openapi/placekey-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Placekey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Placekey secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Placekey
provider_slug: placekey
scheme_count: 1
schemes:
- description: Placekey API key supplied in the apikey request header.
  in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/placekey-openapi.yml
  type: apiKey
slug: placekey-authentication
source_filename: placekey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/placekey-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Placekey API key supplied in the apikey request header.\n  sources:\n  - openapi/placekey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/placekey/refs/heads/main/authentication/placekey-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Location
- Geocoding
- Address Matching
- Identifiers
- POI
---
