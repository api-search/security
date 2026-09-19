---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: astrology-api-astrocartography-api-openapi.yml
  format: yaml
  label: Astrology API Astrocartography API
  slug: astrology-api-astrocartography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-astrocartography-api-openapi.yml
- filename: astrology-api-face-reading-api-openapi.yml
  format: yaml
  label: Astrology API Face Reading API
  slug: astrology-api-face-reading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-face-reading-api-openapi.yml
- filename: astrology-api-human-design-api-openapi.yml
  format: yaml
  label: Astrology API Human Design API
  slug: astrology-api-human-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-human-design-api-openapi.yml
- filename: astrology-api-palm-reading-api-openapi.yml
  format: yaml
  label: Astrology API Palm Reading API
  slug: astrology-api-palm-reading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-palm-reading-api-openapi.yml
- filename: astrology-api-palmistry-service-api-api-openapi.yml
  format: yaml
  label: Astrology API Palmistry Service API
  slug: astrology-api-palmistry-service-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-palmistry-service-api-api-openapi.yml
- filename: astrology-api-pdf-reports-api-openapi.yml
  format: yaml
  label: Astrology API PDF Reports API
  slug: astrology-api-pdf-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-pdf-reports-api-openapi.yml
- filename: astrology-api-prediction-api-openapi.yml
  format: yaml
  label: Astrology API Prediction API
  slug: astrology-api-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-prediction-api-openapi.yml
- filename: astrology-api-vedic-astrology-api-openapi.yml
  format: yaml
  label: Astrology API Vedic Astrology API
  slug: astrology-api-vedic-astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-vedic-astrology-api-openapi.yml
- filename: astrology-api-western-astrology-api-openapi.yml
  format: yaml
  label: Astrology API Western Astrology API
  slug: astrology-api-western-astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-western-astrology-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Astrology Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Astrology API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Astrology API
provider_slug: astrology-api
scheme_count: 2
schemes:
- description: HTTP Basic authentication. Username is your AstrologyAPI User ID, password is your API key. Used with form-encoded request bodies on subscription endpoints.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/astrology-api-json-openapi.yml
  - openapi/astrology-api-pdf-openapi.yml
  - openapi/astrology-api-vision-openapi.yml
  type: http
- description: Wallet Access Token sent in the x-astrologyapi-key header, used with JSON request bodies on wallet-billed and Chat endpoints.
  in: header
  name: accessToken
  parameter: x-astrologyapi-key
  sources:
  - openapi/astrology-api-json-openapi.yml
  - openapi/astrology-api-pdf-openapi.yml
  - openapi/astrology-api-vision-openapi.yml
  type: apiKey
slug: astrology-api-authentication
source_filename: astrology-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/astrology-api-json-openapi.yml, openapi/astrology-api-pdf-openapi.yml, openapi/astrology-api-vision-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Username is your AstrologyAPI User ID, password is\n    your API key. Used with form-encoded request bodies on subscription endpoints.\n  sources:\n  - openapi/astrology-api-json-openapi.yml\n  - openapi/astrology-api-pdf-openapi.yml\n  - openapi/astrology-api-vision-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: x-astrologyapi-key\n  description: Wallet Access Token sent in the x-astrologyapi-key header, used with JSON request\n    bodies on wallet-billed and Chat endpoints.\n  sources:\n  - openapi/astrology-api-json-openapi.yml\n  - openapi/astrology-api-pdf-openapi.yml\n  - openapi/astrology-api-vision-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/authentication/astrology-api-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Astrology
- Horoscopes
- Zodiac
- Vedic Astrology
- Western Astrology
- Kundli
- Panchang
- Numerology
- Tarot
- Palmistry
- Human Design
- Astrocartography
- PDF Reports
- MCP
- Ephemeris
---
