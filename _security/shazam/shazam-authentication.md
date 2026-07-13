---
api_key_in:
- header
api_specs:
- filename: shazam-rest-api-openapi.yml
  format: yaml
  label: Shazam REST API (RapidAPI)
  slug: shazam-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shazam/refs/heads/main/openapi/shazam-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shazam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shazam secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shazam
provider_slug: shazam
scheme_count: 2
schemes:
- description: RapidAPI key for the apidojo/shazam endpoint on rapidapi.com
  in: header
  name: RapidAPIKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/shazam-rest-api-openapi.yml
  type: apiKey
- description: Internal Shazam platform identifier (e.g. IPHONE)
  in: header
  name: ShazamPlatformHeader
  parameter: X-Shazam-Platform
  sources:
  - openapi/shazam-rest-api-openapi.yml
  type: apiKey
slug: shazam-authentication
source_filename: shazam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shazam-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RapidAPIKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: RapidAPI key for the apidojo/shazam endpoint on rapidapi.com\n  sources:\n  - openapi/shazam-rest-api-openapi.yml\n- name: ShazamPlatformHeader\n  type: apiKey\n  in: header\n  parameter: X-Shazam-Platform\n  description: Internal Shazam platform identifier (e.g. IPHONE)\n  sources:\n  - openapi/shazam-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shazam/refs/heads/main/authentication/shazam-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Music
- Audio Recognition
- Song Identification
- Charts
- Artists
- Tracks
- Fingerprinting
---
