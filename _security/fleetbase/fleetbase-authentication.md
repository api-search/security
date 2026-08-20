---
api_key_in: []
api_specs:
- filename: fleetbase-contacts-api-openapi.yml
  format: yaml
  label: Fleetbase Contacts API
  slug: fleetbase-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-contacts-api-openapi.yml
- filename: fleetbase-drivers-api-openapi.yml
  format: yaml
  label: Fleetbase Drivers API
  slug: fleetbase-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-drivers-api-openapi.yml
- filename: fleetbase-fleets-api-openapi.yml
  format: yaml
  label: Fleetbase Fleets API
  slug: fleetbase-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-fleets-api-openapi.yml
- filename: fleetbase-orders-api-openapi.yml
  format: yaml
  label: Fleetbase Orders API
  slug: fleetbase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-orders-api-openapi.yml
- filename: fleetbase-places-api-openapi.yml
  format: yaml
  label: Fleetbase Places API
  slug: fleetbase-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-places-api-openapi.yml
- filename: fleetbase-service-rates-api-openapi.yml
  format: yaml
  label: Fleetbase Service Rates API
  slug: fleetbase-service-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-service-rates-api-openapi.yml
- filename: fleetbase-tracking-api-openapi.yml
  format: yaml
  label: Fleetbase Tracking API
  slug: fleetbase-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-tracking-api-openapi.yml
- filename: fleetbase-vehicles-api-openapi.yml
  format: yaml
  label: Fleetbase Vehicles API
  slug: fleetbase-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-vehicles-api-openapi.yml
- filename: fleetbase-webhooks-api-openapi.yml
  format: yaml
  label: Fleetbase Webhooks API
  slug: fleetbase-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-webhooks-api-openapi.yml
- filename: fleetbase-zones-api-openapi.yml
  format: yaml
  label: Fleetbase Zones API
  slug: fleetbase-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetbase/refs/heads/main/openapi/fleetbase-zones-api-openapi.yml
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
- Open-Source
---
