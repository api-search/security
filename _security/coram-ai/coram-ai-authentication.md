---
api_key_in:
- header
api_specs:
- filename: coram-ai-alerts-api-openapi.yml
  format: yaml
  label: Coram Ai alerts API
  slug: coram-ai-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/openapi/coram-ai-alerts-api-openapi.yml
- filename: coram-ai-camera-groups-api-openapi.yml
  format: yaml
  label: Coram Ai camera-groups API
  slug: coram-ai-camera-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/openapi/coram-ai-camera-groups-api-openapi.yml
- filename: coram-ai-cameras-api-openapi.yml
  format: yaml
  label: Coram Ai cameras API
  slug: coram-ai-cameras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/openapi/coram-ai-cameras-api-openapi.yml
- filename: coram-ai-doors-api-openapi.yml
  format: yaml
  label: Coram Ai doors API
  slug: coram-ai-doors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/openapi/coram-ai-doors-api-openapi.yml
- filename: coram-ai-events-api-openapi.yml
  format: yaml
  label: Coram Ai events API
  slug: coram-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/openapi/coram-ai-events-api-openapi.yml
- filename: coram-ai-locations-api-openapi.yml
  format: yaml
  label: Coram Ai locations API
  slug: coram-ai-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/openapi/coram-ai-locations-api-openapi.yml
- filename: coram-ai-nvrs-api-openapi.yml
  format: yaml
  label: Coram Ai nvrs API
  slug: coram-ai-nvrs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/openapi/coram-ai-nvrs-api-openapi.yml
- filename: coram-ai-reunification-api-openapi.yml
  format: yaml
  label: Coram Ai reunification API
  slug: coram-ai-reunification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/openapi/coram-ai-reunification-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coram Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coram Ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coram Ai
provider_slug: coram-ai
scheme_count: 1
schemes:
- in: header
  name: X-Auth-Token
  parameter: X-Auth-Token
  sources:
  - openapi/coram-ai-openapi-original.json
  type: apiKey
slug: coram-ai-authentication
source_filename: coram-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/coram-ai-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-Auth-Token\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/coram-ai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coram-ai/refs/heads/main/authentication/coram-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Physical Security
- Video Surveillance
- Access Control
- Artificial Intelligence
- Security Cameras
- Emergency Management
- Computer Vision
---
