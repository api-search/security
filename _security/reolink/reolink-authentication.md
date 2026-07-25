---
api_key_in:
- query
api_specs:
- filename: reolink-ai-api-openapi.yml
  format: yaml
  label: Reolink AI API
  slug: reolink-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-ai-api-openapi.yml
- filename: reolink-alarm-api-openapi.yml
  format: yaml
  label: Reolink Alarm API
  slug: reolink-alarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-alarm-api-openapi.yml
- filename: reolink-authentication-api-openapi.yml
  format: yaml
  label: Reolink Authentication API
  slug: reolink-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-authentication-api-openapi.yml
- filename: reolink-encoding-api-openapi.yml
  format: yaml
  label: Reolink Encoding API
  slug: reolink-encoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-encoding-api-openapi.yml
- filename: reolink-led-api-openapi.yml
  format: yaml
  label: Reolink LED API
  slug: reolink-led-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-led-api-openapi.yml
- filename: reolink-network-api-openapi.yml
  format: yaml
  label: Reolink Network API
  slug: reolink-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-network-api-openapi.yml
- filename: reolink-ptz-api-openapi.yml
  format: yaml
  label: Reolink PTZ API
  slug: reolink-ptz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-ptz-api-openapi.yml
- filename: reolink-recording-api-openapi.yml
  format: yaml
  label: Reolink Recording API
  slug: reolink-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-recording-api-openapi.yml
- filename: reolink-security-api-openapi.yml
  format: yaml
  label: Reolink Security API
  slug: reolink-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-security-api-openapi.yml
- filename: reolink-system-api-openapi.yml
  format: yaml
  label: Reolink System API
  slug: reolink-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-system-api-openapi.yml
- filename: reolink-video-api-openapi.yml
  format: yaml
  label: Reolink Video API
  slug: reolink-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/openapi/reolink-video-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reolink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reolink secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reolink
provider_slug: reolink
scheme_count: 1
schemes:
- description: Authentication token obtained from the Login command. Pass as a query parameter on all requests after authentication.
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/reolink-camera-api-openapi.yml
  type: apiKey
slug: reolink-authentication
source_filename: reolink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reolink-camera-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: Authentication token obtained from the Login command. Pass as a query parameter\n    on all requests after authentication.\n  sources:\n  - openapi/reolink-camera-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/authentication/reolink-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
---
