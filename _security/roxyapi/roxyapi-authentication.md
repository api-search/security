---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: roxyapi-angel-numbers-api-openapi.yml
  format: yaml
  label: RoxyAPI Angel Numbers API
  slug: roxyapi-angel-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-angel-numbers-api-openapi.yml
- filename: roxyapi-biorhythm-api-openapi.yml
  format: yaml
  label: RoxyAPI Biorhythm API
  slug: roxyapi-biorhythm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-biorhythm-api-openapi.yml
- filename: roxyapi-chinese-astrology-api-openapi.yml
  format: yaml
  label: RoxyAPI Chinese Astrology API
  slug: roxyapi-chinese-astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-chinese-astrology-api-openapi.yml
- filename: roxyapi-crystals-and-healing-stones-api-openapi.yml
  format: yaml
  label: RoxyAPI Crystals and Healing Stones API
  slug: roxyapi-crystals-and-healing-stones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-crystals-and-healing-stones-api-openapi.yml
- filename: roxyapi-dreams-api-openapi.yml
  format: yaml
  label: RoxyAPI Dreams API
  slug: roxyapi-dreams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-dreams-api-openapi.yml
- filename: roxyapi-feng-shui-api-openapi.yml
  format: yaml
  label: RoxyAPI Feng Shui API
  slug: roxyapi-feng-shui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-feng-shui-api-openapi.yml
- filename: roxyapi-forecast-api-openapi.yml
  format: yaml
  label: RoxyAPI Forecast API
  slug: roxyapi-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-forecast-api-openapi.yml
- filename: roxyapi-human-design-api-openapi.yml
  format: yaml
  label: RoxyAPI Human Design API
  slug: roxyapi-human-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-human-design-api-openapi.yml
- filename: roxyapi-i-ching-api-openapi.yml
  format: yaml
  label: RoxyAPI I Ching API
  slug: roxyapi-i-ching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-i-ching-api-openapi.yml
- filename: roxyapi-languages-api-openapi.yml
  format: yaml
  label: RoxyAPI Languages API
  slug: roxyapi-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-languages-api-openapi.yml
- filename: roxyapi-location-and-timezone-api-openapi.yml
  format: yaml
  label: RoxyAPI Location and Timezone API
  slug: roxyapi-location-and-timezone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-location-and-timezone-api-openapi.yml
- filename: roxyapi-numerology-api-openapi.yml
  format: yaml
  label: RoxyAPI Numerology API
  slug: roxyapi-numerology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-numerology-api-openapi.yml
- filename: roxyapi-tarot-api-openapi.yml
  format: yaml
  label: RoxyAPI Tarot API
  slug: roxyapi-tarot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-tarot-api-openapi.yml
- filename: roxyapi-usage-api-openapi.yml
  format: yaml
  label: RoxyAPI Usage API
  slug: roxyapi-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-usage-api-openapi.yml
- filename: roxyapi-vedic-astrology-api-openapi.yml
  format: yaml
  label: RoxyAPI Vedic Astrology API
  slug: roxyapi-vedic-astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-vedic-astrology-api-openapi.yml
- filename: roxyapi-western-astrology-api-openapi.yml
  format: yaml
  label: RoxyAPI Western Astrology API
  slug: roxyapi-western-astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/openapi/roxyapi-western-astrology-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Roxyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: RoxyAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RoxyAPI
provider_slug: roxyapi
scheme_count: 1
schemes:
- description: Your API key for accessing RoxyAPI. Alternatively, you can pass the API key as a query parameter "api_key".
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/roxyapi-openapi-original.json
  type: apiKey
slug: roxyapi-authentication
source_filename: roxyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/roxyapi-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your API key for accessing RoxyAPI. Alternatively, you can pass the API key as\n    a query parameter \"api_key\".\n  sources:\n  - openapi/roxyapi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/authentication/roxyapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Astrology
- Vedic Astrology
- Numerology
- Tarot
- Human Design
- Forecast
- Biorhythm
- I-Ching
- crystals
- Dreams
- Angel Numbers
- Location
- spiritual
- Wellness
- MCP Server
- OpenAPI
- llms-txt
- Agent-Native
- A2A
---
