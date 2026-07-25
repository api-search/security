---
api_key_in: []
api_specs:
- filename: toyota-climate-api-openapi.yml
  format: yaml
  label: Toyota Climate API
  slug: toyota-climate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-climate-api-openapi.yml
- filename: toyota-electric-api-openapi.yml
  format: yaml
  label: Toyota Electric API
  slug: toyota-electric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-electric-api-openapi.yml
- filename: toyota-fleet-api-openapi.yml
  format: yaml
  label: Toyota Fleet API
  slug: toyota-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-fleet-api-openapi.yml
- filename: toyota-health-api-openapi.yml
  format: yaml
  label: Toyota Health API
  slug: toyota-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-health-api-openapi.yml
- filename: toyota-history-api-openapi.yml
  format: yaml
  label: Toyota History API
  slug: toyota-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-history-api-openapi.yml
- filename: toyota-location-api-openapi.yml
  format: yaml
  label: Toyota Location API
  slug: toyota-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-location-api-openapi.yml
- filename: toyota-notifications-api-openapi.yml
  format: yaml
  label: Toyota Notifications API
  slug: toyota-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-notifications-api-openapi.yml
- filename: toyota-remote-api-openapi.yml
  format: yaml
  label: Toyota Remote API
  slug: toyota-remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-remote-api-openapi.yml
- filename: toyota-status-api-openapi.yml
  format: yaml
  label: Toyota Status API
  slug: toyota-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-status-api-openapi.yml
- filename: toyota-subscriptions-api-openapi.yml
  format: yaml
  label: Toyota Subscriptions API
  slug: toyota-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-subscriptions-api-openapi.yml
- filename: toyota-telemetry-api-openapi.yml
  format: yaml
  label: Toyota Telemetry API
  slug: toyota-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-telemetry-api-openapi.yml
- filename: toyota-trips-api-openapi.yml
  format: yaml
  label: Toyota Trips API
  slug: toyota-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-trips-api-openapi.yml
- filename: toyota-vehicles-api-openapi.yml
  format: yaml
  label: Toyota Vehicles API
  slug: toyota-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-vehicles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Toyota Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toyota secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Toyota
provider_slug: toyota
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/toyota-connected-services-openapi.yml
  - openapi/toyota-telematics-openapi.yml
  type: http
slug: toyota-authentication
source_filename: toyota-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toyota-connected-services-openapi.yml, openapi/toyota-telematics-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/toyota-connected-services-openapi.yml\n  - openapi/toyota-telematics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/authentication/toyota-authentication.yml
summary_line: http · 1 scheme
tags:
- Automobiles
- Cars
- Vehicles
- Connected Car
- Telematics
- Fleet Management
- Electric Vehicles
---
