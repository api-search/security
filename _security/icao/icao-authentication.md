---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: icao-geo-api-openapi.yml
  format: yaml
  label: ICAO GEO API
  slug: icao-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-geo-api-openapi.yml
- filename: icao-icao-api-openapi.yml
  format: yaml
  label: ICAO ICAO API
  slug: icao-icao-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-icao-api-openapi.yml
- filename: icao-infomation-api-openapi.yml
  format: yaml
  label: ICAO Infomation API
  slug: icao-infomation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-infomation-api-openapi.yml
- filename: icao-publication-api-openapi.yml
  format: yaml
  label: ICAO Publication API
  slug: icao-publication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-publication-api-openapi.yml
- filename: icao-safety-api-openapi.yml
  format: yaml
  label: ICAO Safety API
  slug: icao-safety-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-safety-api-openapi.yml
- filename: icao-usoap-api-openapi.yml
  format: yaml
  label: ICAO USOAP API
  slug: icao-usoap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-usoap-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Icao Authentication
name_suffix: Authentication
oauth_flows: []
overview: ICAO secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ICAO
provider_slug: icao
scheme_count: 2
schemes:
- description: Pass api key in URL query parameter.
  in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/icao-openapi.yml
  type: apiKey
- bearerFormat: api_key
  description: Pass api key as Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/icao-openapi.yml
  type: http
slug: icao-authentication
source_filename: icao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/icao-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Pass api key in URL query parameter.\n  sources:\n  - openapi/icao-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: api_key\n  description: Pass api key as Bearer token.\n  sources:\n  - openapi/icao-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/authentication/icao-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Airlines
- Airports
- Airspace
- Aviation
- Reference Data
- Standards
- United Nations
---
