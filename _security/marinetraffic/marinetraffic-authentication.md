---
api_key_in:
- query
api_specs:
- filename: marinetraffic-ais-openapi.yml
  format: yaml
  label: MarineTraffic AIS Vessel Tracking API
  slug: marinetraffic-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-ais-openapi.yml
- filename: marinetraffic-ais-openapi.yml
  format: yaml
  label: MarineTraffic AIS Vessel Tracking API
  slug: marinetraffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-ais-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Marinetraffic Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarineTraffic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarineTraffic
provider_slug: marinetraffic
scheme_count: 1
schemes:
- description: MarineTraffic API key provided in the URL path for most endpoints
  in: query
  name: APIKey
  parameter: apikey
  sources:
  - openapi/marinetraffic-ais-openapi.yml
  type: apiKey
slug: marinetraffic-authentication
source_filename: marinetraffic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marinetraffic-ais-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: APIKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: MarineTraffic API key provided in the URL path for most endpoints\n  sources:\n  - openapi/marinetraffic-ais-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/authentication/marinetraffic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AIS
- Maritime
- Shipping
- Vessel Tracking
---
