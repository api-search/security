---
api_key_in: []
api_specs:
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Places API
  slug: places
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Drivers & Vehicles API
  slug: drivers-vehicles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Fleets & Zones API
  slug: fleets-zones
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Service Rates API
  slug: service-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Tracking API
  slug: tracking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
- filename: fleetbase-openapi.yml
  format: yaml
  label: Fleetbase Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fleetbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fleetbase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fleetbase
provider_slug: fleetbase
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header. Test keys are prefixed flb_test_ and live keys flb_live_.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fleetbase-openapi.yml
  type: http
slug: fleetbase-authentication
source_filename: fleetbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fleetbase-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header. Test keys are prefixed\n    flb_test_ and live keys flb_live_.\n  sources:\n  - openapi/fleetbase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/authentication/fleetbase-authentication.yml
summary_line: http · 1 scheme
tags:
- Logistics
- Fleet Management
- Supply Chain
- Last Mile Delivery
- Open Source
---
