---
anonymous_access: false
api_key_in: []
api_specs:
- filename: audioalpha-io-episode-api-openapi.yml
  format: yaml
  label: AudioAlpha Episode API
  slug: audioalpha-io-episode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-episode-api-openapi.yml
- filename: audioalpha-io-market-api-openapi.yml
  format: yaml
  label: AudioAlpha Market API
  slug: audioalpha-io-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-market-api-openapi.yml
- filename: audioalpha-io-personal-api-openapi.yml
  format: yaml
  label: AudioAlpha Personal API
  slug: audioalpha-io-personal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-personal-api-openapi.yml
- filename: audioalpha-io-podcast-api-openapi.yml
  format: yaml
  label: AudioAlpha Podcast API
  slug: audioalpha-io-podcast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-podcast-api-openapi.yml
- filename: audioalpha-io-ticker-api-openapi.yml
  format: yaml
  label: AudioAlpha Ticker API
  slug: audioalpha-io-ticker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioalpha-io/openapi/audioalpha-io-ticker-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AudioAlpha Authentication
name_suffix: Authentication
oauth_flows: []
overview: AudioAlpha secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AudioAlpha
provider_slug: audioalpha-io
scheme_count: 1
schemes:
- description: API key generated from https://audioalpha.io/account
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/audioalpha-io-openapi.json
  type: http
slug: audioalpha-io-authentication
source_filename: audioalpha-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/audioalpha-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key generated from https://audioalpha.io/account\n  sources:\n  - openapi/audioalpha-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/audioalpha-io/authentication/audioalpha-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Podcasts
- Transcription
- Market Data
- Company
---
