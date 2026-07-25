---
api_key_in:
- header
api_specs:
- filename: loconav-alert-subscriptions-api-openapi.yml
  format: yaml
  label: LocoNav Alert Subscriptions API
  slug: loconav-alert-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-alert-subscriptions-api-openapi.yml
- filename: loconav-alerts-api-openapi.yml
  format: yaml
  label: LocoNav Alerts API
  slug: loconav-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-alerts-api-openapi.yml
- filename: loconav-alerts-subscriptions-api-openapi.yml
  format: yaml
  label: LocoNav Alerts Subscriptions API
  slug: loconav-alerts-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-alerts-subscriptions-api-openapi.yml
- filename: loconav-drivers-api-openapi.yml
  format: yaml
  label: LocoNav Drivers API
  slug: loconav-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-drivers-api-openapi.yml
- filename: loconav-mobilization-api-openapi.yml
  format: yaml
  label: LocoNav Mobilization API
  slug: loconav-mobilization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-mobilization-api-openapi.yml
- filename: loconav-polygon-geofence-api-openapi.yml
  format: yaml
  label: LocoNav Polygon (Geofence) API
  slug: loconav-polygon-geofence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-polygon-geofence-api-openapi.yml
- filename: loconav-trips-api-openapi.yml
  format: yaml
  label: LocoNav Trips API
  slug: loconav-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-trips-api-openapi.yml
- filename: loconav-users-api-openapi.yml
  format: yaml
  label: LocoNav Users API
  slug: loconav-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-users-api-openapi.yml
- filename: loconav-vehicles-api-openapi.yml
  format: yaml
  label: LocoNav Vehicles API
  slug: loconav-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-vehicles-api-openapi.yml
- filename: loconav-vehicles-telematics-api-openapi.yml
  format: yaml
  label: LocoNav Vehicles / Telematics API
  slug: loconav-vehicles-telematics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-vehicles-telematics-api-openapi.yml
- filename: loconav-video-telematics-vt-live-stream-api-openapi.yml
  format: yaml
  label: LocoNav Video Telematics VT / Live Stream API
  slug: loconav-video-telematics-vt-live-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-video-telematics-vt-live-stream-api-openapi.yml
- filename: loconav-video-telematics-vt-videos-api-openapi.yml
  format: yaml
  label: LocoNav Video Telematics VT / Videos API
  slug: loconav-video-telematics-vt-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-video-telematics-vt-videos-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Loconav Authentication
name_suffix: Authentication
oauth_flows: []
overview: LocoNav secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LocoNav
provider_slug: loconav
scheme_count: 1
schemes:
- description: User-level API token supplied in the User-Authentication request header. Each user is assigned a unique auth token, provisioned by a LocoNav SPOC (single point of contact). Incorrect or missing credentials return 401 Unauthorized.
  in: header
  name: UserAuthentication
  parameter: User-Authentication
  sources:
  - openapi/loconav-integration-openapi.yml
  token_provisioning: LocoNav SPOC (manual, per user)
  type: apiKey
slug: loconav-authentication
source_filename: loconav-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/loconav-integration-openapi.yml\ndocs: https://developers.loconav.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: UserAuthentication\n  type: apiKey\n  in: header\n  parameter: User-Authentication\n  description: >-\n    User-level API token supplied in the User-Authentication request header.\n    Each user is assigned a unique auth token, provisioned by a LocoNav SPOC\n    (single point of contact). Incorrect or missing credentials return 401\n    Unauthorized.\n  token_provisioning: LocoNav SPOC (manual, per user)\n  sources:\n  - openapi/loconav-integration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/authentication/loconav-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fleet Management
- Telematics
- GPS Tracking
- Vehicle Tracking
- Transportation
- Logistics
- IoT
- Video Telematics
- Webhooks
---
