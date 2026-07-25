---
api_key_in:
- header
api_specs:
- filename: moon-api-advanced-api-openapi.yml
  format: yaml
  label: Moon-API Advanced API
  slug: moon-api-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/openapi/moon-api-advanced-api-openapi.yml
- filename: moon-api-astrology-api-openapi.yml
  format: yaml
  label: Moon-API Astrology API
  slug: moon-api-astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/openapi/moon-api-astrology-api-openapi.yml
- filename: moon-api-basic-api-openapi.yml
  format: yaml
  label: Moon-API Basic API
  slug: moon-api-basic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/openapi/moon-api-basic-api-openapi.yml
- filename: moon-api-calendar-api-openapi.yml
  format: yaml
  label: Moon-API Calendar API
  slug: moon-api-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/openapi/moon-api-calendar-api-openapi.yml
- filename: moon-api-emoji-api-openapi.yml
  format: yaml
  label: Moon-API Emoji API
  slug: moon-api-emoji-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/openapi/moon-api-emoji-api-openapi.yml
- filename: moon-api-phase-api-openapi.yml
  format: yaml
  label: Moon-API Phase API
  slug: moon-api-phase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/openapi/moon-api-phase-api-openapi.yml
- filename: moon-api-plain-text-api-openapi.yml
  format: yaml
  label: Moon-API Plain Text API
  slug: moon-api-plain-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/openapi/moon-api-plain-text-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Moon Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moon-API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moon-API
provider_slug: moon-api
scheme_count: 1
schemes:
- description: RapidAPI authentication key
  in: header
  name: RapidAPIKey
  parameter: x-rapidapi-key
  sources:
  - openapi/moon-api-openapi.yml
  type: apiKey
slug: moon-api-authentication
source_filename: moon-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moon-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RapidAPIKey\n  type: apiKey\n  in: header\n  parameter: x-rapidapi-key\n  description: RapidAPI authentication key\n  sources:\n  - openapi/moon-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/authentication/moon-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Astrology
- Astronomy
- Lunar
- Moon
- Moon Phases
- Space
---
