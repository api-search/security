---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Steam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Steam secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Steam
provider_slug: steam
scheme_count: 1
schemes:
- description: Steam Web API key. Obtain at https://steamcommunity.com/dev/apikey.
  in: query
  name: ApiKey
  parameter: key
  sources:
  - openapi/steam-openapi.yml
  type: apiKey
slug: steam-authentication
source_filename: steam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/steam-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Steam Web API key. Obtain at https://steamcommunity.com/dev/apikey.\n  sources:\n  - openapi/steam-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steam/refs/heads/main/authentication/steam-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Gaming
- Valve
- Distribution
- Steamworks
- Marketplace
- Web API
---
