---
api_key_in: []
api_specs:
- filename: flightradar24-airlines-api-openapi.yml
  format: yaml
  label: Flightradar24 Airlines API
  slug: flightradar24-airlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-airlines-api-openapi.yml
- filename: flightradar24-airports-api-openapi.yml
  format: yaml
  label: Flightradar24 Airports API
  slug: flightradar24-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-airports-api-openapi.yml
- filename: flightradar24-flight-summary-api-openapi.yml
  format: yaml
  label: Flightradar24 Flight Summary API
  slug: flightradar24-flight-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-flight-summary-api-openapi.yml
- filename: flightradar24-flight-tracks-api-openapi.yml
  format: yaml
  label: Flightradar24 Flight Tracks API
  slug: flightradar24-flight-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-flight-tracks-api-openapi.yml
- filename: flightradar24-historic-events-api-openapi.yml
  format: yaml
  label: Flightradar24 Historic Events API
  slug: flightradar24-historic-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-historic-events-api-openapi.yml
- filename: flightradar24-historic-positions-api-openapi.yml
  format: yaml
  label: Flightradar24 Historic Positions API
  slug: flightradar24-historic-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-historic-positions-api-openapi.yml
- filename: flightradar24-live-positions-api-openapi.yml
  format: yaml
  label: Flightradar24 Live Positions API
  slug: flightradar24-live-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-live-positions-api-openapi.yml
- filename: flightradar24-usage-api-openapi.yml
  format: yaml
  label: Flightradar24 Usage API
  slug: flightradar24-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-usage-api-openapi.yml
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
