---
api_key_in:
- header
api_specs:
- filename: weavix-channels-messaging-api-openapi.yml
  format: yaml
  label: Weavix Channels & Messaging API
  slug: weavix-channels-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-channels-messaging-api-openapi.yml
- filename: weavix-crafts-api-openapi.yml
  format: yaml
  label: Weavix Crafts API
  slug: weavix-crafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-crafts-api-openapi.yml
- filename: weavix-forms-api-openapi.yml
  format: yaml
  label: Weavix Forms API
  slug: weavix-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-forms-api-openapi.yml
- filename: weavix-geofences-api-openapi.yml
  format: yaml
  label: Weavix Geofences API
  slug: weavix-geofences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-geofences-api-openapi.yml
- filename: weavix-mass-alerts-api-openapi.yml
  format: yaml
  label: Weavix Mass Alerts API
  slug: weavix-mass-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-mass-alerts-api-openapi.yml
- filename: weavix-permission-groups-api-openapi.yml
  format: yaml
  label: Weavix Permission Groups API
  slug: weavix-permission-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-permission-groups-api-openapi.yml
- filename: weavix-sites-api-openapi.yml
  format: yaml
  label: Weavix Sites API
  slug: weavix-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-sites-api-openapi.yml
- filename: weavix-user-management-api-openapi.yml
  format: yaml
  label: Weavix User Management API
  slug: weavix-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-user-management-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Weavix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weavix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weavix
provider_slug: weavix
scheme_count: 1
schemes:
- description: Account API key passed as the Authorization request header. Keys are created in the weavix Console under Configuration -> API Keys (Secret + Authorization Token). Requests without a valid token receive 401.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/weavix-rest-openapi.yml
  type: apiKey
slug: weavix-authentication
source_filename: weavix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/weavix-rest-openapi.yml\ndocs: https://help.weavix.com/hc/en-us/articles/45825355414669-Weavix-API-s\nnotes: >-\n  API access must be enabled for the account (contact help@weavix.com). An API\n  key is created in the weavix Console under Configuration -> API Keys, which\n  issues a Secret and an Authorization Token. Every request must send the token\n  in the Authorization header (raw token, no Bearer prefix), e.g.\n  `curl -H \"Authorization: YOUR_AUTHORIZATION_TOKEN\" https://api.weavix.com/v1/core/people`.\n  Requests without a valid token receive HTTP 401.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Account API key passed as the Authorization request header. Keys are created\n    in the weavix Console under Configuration -> API Keys (Secret + Authorization Token). Requests\n    without a valid token\
  \ receive 401.\n  sources:\n  - openapi/weavix-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/authentication/weavix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Communication
- Frontline Workers
- Workforce Management
- Messaging
- Push To Talk
- Industrial
- Internet of Things
- Location Tracking
- Alerts
- Company
---
