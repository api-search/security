---
api_key_in:
- header
api_specs:
- filename: govee-openapi.yml
  format: yaml
  label: Govee Devices API
  slug: govee-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Device State API
  slug: govee-device-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Device Control API
  slug: govee-device-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Dynamic Scenes API
  slug: govee-dynamic-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee DIY Scenes API
  slug: govee-diy-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Segment Color and Brightness API
  slug: govee-segment-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Govee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Govee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Govee
provider_slug: govee
scheme_count: 1
schemes:
- description: API key issued in the Govee Home App (Profile > About Us > Apply for API Key).
  in: header
  name: GoveeApiKey
  parameter: Govee-API-Key
  sources:
  - openapi/govee-openapi.yml
  type: apiKey
slug: govee-authentication
source_filename: govee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/govee-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: GoveeApiKey\n  type: apiKey\n  in: header\n  parameter: Govee-API-Key\n  description: API key issued in the Govee Home App (Profile > About Us > Apply for API Key).\n  sources:\n  - openapi/govee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/authentication/govee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Smart Home
- Smart Lighting
- IoT
- LED
- Home Automation
- Device Control
---
