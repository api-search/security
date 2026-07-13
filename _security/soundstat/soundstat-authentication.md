---
api_key_in:
- header
api_specs:
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Track Analysis API
  slug: soundstat-track-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Search & Discovery API
  slug: soundstat-search-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Recommendations API
  slug: soundstat-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Soundstat Authentication
name_suffix: Authentication
oauth_flows: []
overview: SoundStat secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SoundStat
provider_slug: soundstat
scheme_count: 1
schemes:
- description: API key issued after registration at https://soundstat.info/auth.html. Passed in the x-api-key request header.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/soundstat-openapi.yml
  type: apiKey
slug: soundstat-authentication
source_filename: soundstat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soundstat-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued after registration at https://soundstat.info/auth.html. Passed\n    in the x-api-key request header.\n  sources:\n  - openapi/soundstat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/authentication/soundstat-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Music
- Audio Analysis
- Audio Features
- Recommendations
- Track Analysis
- Spotify Alternative
---
