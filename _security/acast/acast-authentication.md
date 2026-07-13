---
api_key_in:
- header
api_specs:
- filename: acast-openapi.yml
  format: yaml
  label: Acast Shows API
  slug: acast-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acast/refs/heads/main/openapi/acast-openapi.yml
- filename: acast-openapi.yml
  format: yaml
  label: Acast Episodes API
  slug: acast-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acast/refs/heads/main/openapi/acast-openapi.yml
- filename: acast-openapi.yml
  format: yaml
  label: Acast Ad Markers API
  slug: acast-ad-markers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acast/refs/heads/main/openapi/acast-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Acast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Acast
provider_slug: acast
scheme_count: 1
schemes:
- description: User-scoped API key issued by Acast customer success to Ace plan and Creator Network accounts. Sent on every request in the X-API-Key header.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/acast-openapi.yml
  type: apiKey
slug: acast-authentication
source_filename: acast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acast-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: User-scoped API key issued by Acast customer success to Ace plan and Creator\n    Network accounts. Sent on every request in the X-API-Key header.\n  sources:\n  - openapi/acast-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acast/refs/heads/main/authentication/acast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Podcasting
- Podcast Hosting
- Publishing
- Advertising
- Monetization
- Media
- Audio
---
