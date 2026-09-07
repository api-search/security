---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: marine-traffic-ais-api-api-openapi.yml
  format: yaml
  label: MarineTraffic AIS API API
  slug: marine-traffic-ais-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-ais-api-api-openapi.yml
- filename: marine-traffic-balances-api-openapi.yml
  format: yaml
  label: MarineTraffic Balances API
  slug: marine-traffic-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-balances-api-openapi.yml
- filename: marine-traffic-fleets-api-openapi.yml
  format: yaml
  label: MarineTraffic Fleets API
  slug: marine-traffic-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-fleets-api-openapi.yml
- filename: marine-traffic-passage-plans-api-openapi.yml
  format: yaml
  label: MarineTraffic Passage Plans API
  slug: marine-traffic-passage-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-passage-plans-api-openapi.yml
- filename: marine-traffic-port-events-api-openapi.yml
  format: yaml
  label: MarineTraffic Port Events API
  slug: marine-traffic-port-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-port-events-api-openapi.yml
- filename: marine-traffic-ports-information-api-openapi.yml
  format: yaml
  label: MarineTraffic Ports Information API
  slug: marine-traffic-ports-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-ports-information-api-openapi.yml
- filename: marine-traffic-reverse-geocoding-api-openapi.yml
  format: yaml
  label: MarineTraffic Reverse Geocoding API
  slug: marine-traffic-reverse-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-reverse-geocoding-api-openapi.yml
- filename: marine-traffic-routing-information-api-openapi.yml
  format: yaml
  label: MarineTraffic Routing Information API
  slug: marine-traffic-routing-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-routing-information-api-openapi.yml
- filename: marine-traffic-search-vessel-api-openapi.yml
  format: yaml
  label: MarineTraffic Search Vessel API
  slug: marine-traffic-search-vessel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-search-vessel-api-openapi.yml
- filename: marine-traffic-single-vessel-events-api-openapi.yml
  format: yaml
  label: MarineTraffic Single Vessel Events API
  slug: marine-traffic-single-vessel-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-single-vessel-events-api-openapi.yml
- filename: marine-traffic-vessel-historical-track-api-openapi.yml
  format: yaml
  label: MarineTraffic Vessel Historical Track API
  slug: marine-traffic-vessel-historical-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-vessel-historical-track-api-openapi.yml
- filename: marine-traffic-vessel-information-api-openapi.yml
  format: yaml
  label: MarineTraffic Vessel Information API
  slug: marine-traffic-vessel-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-vessel-information-api-openapi.yml
- filename: marine-traffic-vessel-positions-legacy-api-api-openapi.yml
  format: yaml
  label: MarineTraffic Vessel Positions (Legacy API) API
  slug: marine-traffic-vessel-positions-legacy-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-vessel-positions-legacy-api-api-openapi.yml
- filename: marine-traffic-voyage-information-api-openapi.yml
  format: yaml
  label: MarineTraffic Voyage Information API
  slug: marine-traffic-voyage-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/openapi/marine-traffic-voyage-information-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Marine Traffic Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarineTraffic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarineTraffic
provider_slug: marine-traffic
scheme_count: 1
schemes:
- description: MarineTraffic API key provided in the URL path for most endpoints
  in: query
  name: APIKey
  parameter: apikey
  sources:
  - openapi/marinetraffic-ais-openapi.yml
  type: apiKey
slug: marine-traffic-authentication
source_filename: marine-traffic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marinetraffic-ais-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: APIKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: MarineTraffic API key provided in the URL path for most endpoints\n  sources:\n  - openapi/marinetraffic-ais-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marine-traffic/refs/heads/main/authentication/marine-traffic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AIS
- Maritime
- Vessel Tracking
- Shipping
- Ports
- Voyage Forecasting
- Geospatial
- Kpler
---
