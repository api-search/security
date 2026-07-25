---
api_key_in:
- query
api_specs:
- filename: marinetraffic-port-operations-api-openapi.yml
  format: yaml
  label: MarineTraffic Port Operations API
  slug: marinetraffic-port-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-port-operations-api-openapi.yml
- filename: marinetraffic-vessel-tracking-api-openapi.yml
  format: yaml
  label: MarineTraffic Vessel Tracking API
  slug: marinetraffic-vessel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-vessel-tracking-api-openapi.yml
- filename: marinetraffic-vessels-api-openapi.yml
  format: yaml
  label: MarineTraffic Vessels API
  slug: marinetraffic-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-vessels-api-openapi.yml
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
