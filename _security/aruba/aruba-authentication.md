---
api_key_in: []
api_specs:
- filename: aruba-access-points-api-openapi.yml
  format: yaml
  label: Aruba Access Points API
  slug: aruba-access-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/openapi/aruba-access-points-api-openapi.yml
- filename: aruba-devices-api-openapi.yml
  format: yaml
  label: Aruba Devices API
  slug: aruba-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/openapi/aruba-devices-api-openapi.yml
- filename: aruba-groups-api-openapi.yml
  format: yaml
  label: Aruba Groups API
  slug: aruba-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/openapi/aruba-groups-api-openapi.yml
- filename: aruba-monitoring-api-openapi.yml
  format: yaml
  label: Aruba Monitoring API
  slug: aruba-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/openapi/aruba-monitoring-api-openapi.yml
- filename: aruba-sites-api-openapi.yml
  format: yaml
  label: Aruba Sites API
  slug: aruba-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/openapi/aruba-sites-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aruba Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aruba secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aruba
provider_slug: aruba
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained through the Aruba Central API Gateway three-step OAuth flow. Tokens expire after 7200 seconds (2 hours) and can be refreshed using the refresh_token grant type.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aruba-central-api.yml
  type: http
slug: aruba-authentication
source_filename: aruba-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aruba-central-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained through the Aruba Central API Gateway three-step\n    OAuth flow. Tokens expire after 7200 seconds (2 hours) and can be refreshed using the refresh_token\n    grant type.\n  sources:\n  - openapi/aruba-central-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/authentication/aruba-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
---
