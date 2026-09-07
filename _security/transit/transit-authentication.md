---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: transit-alerts-api-openapi.yml
  format: yaml
  label: Transit Alerts API
  slug: transit-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-alerts-api-openapi.yml
- filename: transit-departures-api-openapi.yml
  format: yaml
  label: Transit Departures API
  slug: transit-departures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-departures-api-openapi.yml
- filename: transit-mobility-api-openapi.yml
  format: yaml
  label: Transit Mobility API
  slug: transit-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-mobility-api-openapi.yml
- filename: transit-networks-api-openapi.yml
  format: yaml
  label: Transit Networks API
  slug: transit-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-networks-api-openapi.yml
- filename: transit-routes-api-openapi.yml
  format: yaml
  label: Transit Routes API
  slug: transit-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-routes-api-openapi.yml
- filename: transit-stops-api-openapi.yml
  format: yaml
  label: Transit Stops API
  slug: transit-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-stops-api-openapi.yml
- filename: transit-trips-api-openapi.yml
  format: yaml
  label: Transit Trips API
  slug: transit-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-trips-api-openapi.yml
- filename: transitapp-locations-api-openapi.yml
  format: yaml
  label: Transit Locations API
  slug: transitapp-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transitapp-locations-api-openapi.yml
- filename: transitapp-nearby-routes-api-openapi.yml
  format: yaml
  label: Transit Nearby Routes API
  slug: transitapp-nearby-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transitapp-nearby-routes-api-openapi.yml
- filename: transitapp-nearby-stops-api-openapi.yml
  format: yaml
  label: Transit Nearby Stops API
  slug: transitapp-nearby-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transitapp-nearby-stops-api-openapi.yml
- filename: transitapp-route-details-api-openapi.yml
  format: yaml
  label: Transit Route Details API
  slug: transitapp-route-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transitapp-route-details-api-openapi.yml
- filename: transitapp-service-alerts-api-openapi.yml
  format: yaml
  label: Transit Service Alerts API
  slug: transitapp-service-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transitapp-service-alerts-api-openapi.yml
- filename: transitapp-stop-departures-api-openapi.yml
  format: yaml
  label: Transit Stop Departures API
  slug: transitapp-stop-departures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transitapp-stop-departures-api-openapi.yml
- filename: transitapp-trip-planning-api-openapi.yml
  format: yaml
  label: Transit Trip Planning API
  slug: transitapp-trip-planning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transitapp-trip-planning-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Transit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transit
provider_slug: transit
scheme_count: 1
schemes:
- description: API key provided after partner approval
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/transit-openapi.yml
  type: apiKey
slug: transit-authentication
source_filename: transit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/transit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key provided after partner approval\n  sources:\n  - openapi/transit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/authentication/transit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Public Transit
- Real-Time
- Trip Planning
- Multi-Modal
- GTFS
- GOFS
- Mobility
- Shared Mobility
---
