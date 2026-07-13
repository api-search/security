---
api_key_in: []
api_specs:
- filename: tive-openapi.yml
  format: yaml
  label: Tive Shipments API
  slug: tive-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
- filename: tive-openapi.yml
  format: yaml
  label: Tive Trackers / Devices API
  slug: tive-trackers-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
- filename: tive-openapi.yml
  format: yaml
  label: Tive Sensor Data API
  slug: tive-sensor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
- filename: tive-openapi.yml
  format: yaml
  label: Tive Alerts API
  slug: tive-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
- filename: tive-openapi.yml
  format: yaml
  label: Tive Webhooks API
  slug: tive-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/openapi/tive-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tive
provider_slug: tive
scheme_count: 1
schemes:
- description: 'Bearer token obtained from POST /authenticate. Send it as ''Authorization: Bearer <token>''. Most endpoints additionally require the x-tive-account-id header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tive-openapi.yml
  type: http
slug: tive-authentication
source_filename: tive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tive-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token obtained from POST /authenticate. Send it as ''Authorization: Bearer\n    <token>''. Most endpoints additionally require the x-tive-account-id header.'\n  sources:\n  - openapi/tive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tive/refs/heads/main/authentication/tive-authentication.yml
summary_line: http · 1 scheme
tags:
- Supply Chain
- Shipment Visibility
- Logistics
- IoT
- Trackers
- Real Time
---
