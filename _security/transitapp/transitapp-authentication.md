---
api_key_in:
- header
api_specs:
- filename: transitapp-openapi.yml
  format: yaml
  label: Transit Nearby Routes API
  slug: transitapp-nearby-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitapp/refs/heads/main/openapi/transitapp-openapi.yml
- filename: transitapp-openapi.yml
  format: yaml
  label: Transit Nearby Stops API
  slug: transitapp-nearby-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitapp/refs/heads/main/openapi/transitapp-openapi.yml
- filename: transitapp-openapi.yml
  format: yaml
  label: Transit Stop Departures API
  slug: transitapp-stop-departures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitapp/refs/heads/main/openapi/transitapp-openapi.yml
- filename: transitapp-openapi.yml
  format: yaml
  label: Transit Route Details API
  slug: transitapp-route-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitapp/refs/heads/main/openapi/transitapp-openapi.yml
- filename: transitapp-openapi.yml
  format: yaml
  label: Transit Trip Planning API
  slug: transitapp-trip-planning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitapp/refs/heads/main/openapi/transitapp-openapi.yml
- filename: transitapp-openapi.yml
  format: yaml
  label: Transit Service Alerts API
  slug: transitapp-service-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitapp/refs/heads/main/openapi/transitapp-openapi.yml
- filename: transitapp-openapi.yml
  format: yaml
  label: Transit Locations API
  slug: transitapp-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitapp/refs/heads/main/openapi/transitapp-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Transitapp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transit
provider_slug: transitapp
scheme_count: 1
schemes:
- description: Transit access key requested via Transit's API request form. Sent as the `apiKey` request header on every call.
  in: header
  name: apiKeyAuth
  parameter: apiKey
  sources:
  - openapi/transitapp-openapi.yml
  type: apiKey
slug: transitapp-authentication
source_filename: transitapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/transitapp-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: Transit access key requested via Transit's API request form. Sent as the `apiKey`\n    request header on every call.\n  sources:\n  - openapi/transitapp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transitapp/refs/heads/main/authentication/transitapp-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Transit
- Public Transportation
- Real-Time
- Mobility
- Trip Planning
- Departures
- GTFS
- MaaS
---
