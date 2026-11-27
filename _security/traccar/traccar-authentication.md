---
anonymous_access: false
api_key_in: []
api_specs:
- filename: traccar-attributes-api-openapi.yml
  format: yaml
  label: Traccar Attributes API
  slug: traccar-attributes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-attributes-api-openapi.yml
- filename: traccar-audit-api-openapi.yml
  format: yaml
  label: Traccar Audit API
  slug: traccar-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-audit-api-openapi.yml
- filename: traccar-calendars-api-openapi.yml
  format: yaml
  label: Traccar Calendars API
  slug: traccar-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-calendars-api-openapi.yml
- filename: traccar-commands-api-openapi.yml
  format: yaml
  label: Traccar Commands API
  slug: traccar-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-commands-api-openapi.yml
- filename: traccar-devices-api-openapi.yml
  format: yaml
  label: Traccar Devices API
  slug: traccar-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-devices-api-openapi.yml
- filename: traccar-drivers-api-openapi.yml
  format: yaml
  label: Traccar Drivers API
  slug: traccar-drivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-drivers-api-openapi.yml
- filename: traccar-events-api-openapi.yml
  format: yaml
  label: Traccar Events API
  slug: traccar-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-events-api-openapi.yml
- filename: traccar-geofences-api-openapi.yml
  format: yaml
  label: Traccar Geofences API
  slug: traccar-geofences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-geofences-api-openapi.yml
- filename: traccar-groups-api-openapi.yml
  format: yaml
  label: Traccar Groups API
  slug: traccar-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-groups-api-openapi.yml
- filename: traccar-health-api-openapi.yml
  format: yaml
  label: Traccar Health API
  slug: traccar-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-health-api-openapi.yml
- filename: traccar-maintenance-api-openapi.yml
  format: yaml
  label: Traccar Maintenance API
  slug: traccar-maintenance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-maintenance-api-openapi.yml
- filename: traccar-notifications-api-openapi.yml
  format: yaml
  label: Traccar Notifications API
  slug: traccar-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-notifications-api-openapi.yml
- filename: traccar-orders-api-openapi.yml
  format: yaml
  label: Traccar Orders API
  slug: traccar-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-orders-api-openapi.yml
- filename: traccar-password-api-openapi.yml
  format: yaml
  label: Traccar Password API
  slug: traccar-password-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-password-api-openapi.yml
- filename: traccar-permissions-api-openapi.yml
  format: yaml
  label: Traccar Permissions API
  slug: traccar-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-permissions-api-openapi.yml
- filename: traccar-positions-api-openapi.yml
  format: yaml
  label: Traccar Positions API
  slug: traccar-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-positions-api-openapi.yml
- filename: traccar-reports-api-openapi.yml
  format: yaml
  label: Traccar Reports API
  slug: traccar-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-reports-api-openapi.yml
- filename: traccar-server-api-openapi.yml
  format: yaml
  label: Traccar Server API
  slug: traccar-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-server-api-openapi.yml
- filename: traccar-session-api-openapi.yml
  format: yaml
  label: Traccar Session API
  slug: traccar-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-session-api-openapi.yml
- filename: traccar-share-api-openapi.yml
  format: yaml
  label: Traccar Share API
  slug: traccar-share-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-share-api-openapi.yml
- filename: traccar-statistics-api-openapi.yml
  format: yaml
  label: Traccar Statistics API
  slug: traccar-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-statistics-api-openapi.yml
- filename: traccar-stream-api-openapi.yml
  format: yaml
  label: Traccar Stream API
  slug: traccar-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-stream-api-openapi.yml
- filename: traccar-users-api-openapi.yml
  format: yaml
  label: Traccar Users API
  slug: traccar-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/traccar/openapi/traccar-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Traccar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Traccar secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Traccar
provider_slug: traccar
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/traccar-openapi.yaml
  type: http
- name: ApiKey
  scheme: bearer
  sources:
  - openapi/traccar-openapi.yaml
  type: http
slug: traccar-authentication
source_filename: traccar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/traccar-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/traccar-openapi.yaml\n- name: ApiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/traccar-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/traccar/authentication/traccar-authentication.yml
summary_line: http · 2 schemes
tags:
- GPS Tracking
- Open-source software
- Managed Hosting
---
