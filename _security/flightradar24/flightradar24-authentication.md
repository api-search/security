---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Flightradar24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flightradar24 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flightradar24
provider_slug: flightradar24
scheme_count: 1
schemes:
- description: Bearer token authentication. Obtain your API token from the Flightradar24 developer portal at https://fr24api.flightradar24.com/.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: flightradar24-authentication
source_filename: flightradar24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Obtain your API token from the Flightradar24 developer\n    portal at https://fr24api.flightradar24.com/.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/authentication/flightradar24-authentication.yml
summary_line: http · 1 scheme
tags:
- Aviation
- Flight Tracking
- Real-Time
- Aircraft
- Airports
- Airlines
- ADS-B
- Historical Data
---
