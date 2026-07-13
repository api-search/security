---
api_key_in:
- header
api_specs:
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Artists API
  slug: setlistfm-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Setlists API
  slug: setlistfm-setlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Venues API
  slug: setlistfm-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Cities API
  slug: setlistfm-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Countries API
  slug: setlistfm-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Search API
  slug: setlistfm-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm User API
  slug: setlistfm-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Setlistfm Authentication
name_suffix: Authentication
oauth_flows: []
overview: setlist.fm secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: setlist.fm
provider_slug: setlistfm
scheme_count: 1
schemes:
- description: API key issued from https://www.setlist.fm/settings/api. Passed in the `x-api-key` request header on every call.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/setlistfm-openapi.yml
  type: apiKey
slug: setlistfm-authentication
source_filename: setlistfm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/setlistfm-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued from https://www.setlist.fm/settings/api. Passed in the `x-api-key`\n    request header on every call.\n  sources:\n  - openapi/setlistfm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/authentication/setlistfm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Music
- Concerts
- Setlists
- Live Music
- Database
- Crowd-Sourced
- Entertainment
---
