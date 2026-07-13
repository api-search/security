---
api_key_in: []
api_specs:
- filename: trimble-mobile-manager-openapi.yml
  format: yaml
  label: Trimble Mobile Manager API
  slug: trimble-mobile-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/openapi/trimble-mobile-manager-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trimble Navigation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trimble Navigation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trimble Navigation
provider_slug: trimble-navigation
scheme_count: 1
schemes:
- description: Access code generated using SHA256 hash of (applicationId + currentUTCTime), Base64 encoded. Valid for 1 second only. Must be regenerated per request.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/trimble-mobile-manager-openapi.yml
  type: http
slug: trimble-navigation-authentication
source_filename: trimble-navigation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trimble-mobile-manager-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Access code generated using SHA256 hash of (applicationId + currentUTCTime),\n    Base64 encoded. Valid for 1 second only. Must be regenerated per request.\n  sources:\n  - openapi/trimble-mobile-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/authentication/trimble-navigation-authentication.yml
summary_line: http · 1 scheme
tags:
- GPS
- GNSS
- Positioning
- Navigation
- Surveying
- Geospatial
- Construction
- Fortune 1000
---
