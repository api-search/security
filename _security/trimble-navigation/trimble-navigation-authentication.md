---
api_key_in: []
api_specs:
- filename: trimble-navigation-catalyst-api-openapi.yml
  format: yaml
  label: Trimble Navigation Catalyst API
  slug: trimble-navigation-catalyst-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/openapi/trimble-navigation-catalyst-api-openapi.yml
- filename: trimble-navigation-corrections-api-openapi.yml
  format: yaml
  label: Trimble Navigation Corrections API
  slug: trimble-navigation-corrections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/openapi/trimble-navigation-corrections-api-openapi.yml
- filename: trimble-navigation-positioning-api-openapi.yml
  format: yaml
  label: Trimble Navigation Positioning API
  slug: trimble-navigation-positioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/openapi/trimble-navigation-positioning-api-openapi.yml
- filename: trimble-navigation-receiver-api-openapi.yml
  format: yaml
  label: Trimble Navigation Receiver API
  slug: trimble-navigation-receiver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/openapi/trimble-navigation-receiver-api-openapi.yml
- filename: trimble-navigation-system-api-openapi.yml
  format: yaml
  label: Trimble Navigation System API
  slug: trimble-navigation-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/openapi/trimble-navigation-system-api-openapi.yml
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
