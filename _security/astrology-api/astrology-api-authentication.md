---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: astrology-api-json-openapi.yml
  format: yaml
  label: Astrology API
  slug: astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-json-openapi.yml
- filename: astrology-api-pdf-openapi.yml
  format: yaml
  label: AstrologyAPI PDF Reports API
  slug: astrology-api-pdf
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-pdf-openapi.yml
- filename: astrology-api-palmistry-openapi.json
  format: json
  label: AstrologyAPI Palmistry API
  slug: astrology-api-palmistry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-palmistry-openapi.json
- filename: astrology-api-face-reading-openapi.yml
  format: yaml
  label: AstrologyAPI Face Reading API
  slug: astrology-api-face-reading
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-face-reading-openapi.yml
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
