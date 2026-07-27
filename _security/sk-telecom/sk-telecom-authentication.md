---
api_key_in:
- header
api_specs:
- filename: sk-telecom-ax-tts-openapi.json
  format: json
  label: SK Telecom A.X TTS API
  slug: sk-telecom-ax-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-ax-tts-openapi.json
- filename: sk-telecom-facecan-openapi.json
  format: json
  label: SK Telecom A. facecan API
  slug: sk-telecom-facecan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-facecan-openapi.json
- filename: sk-telecom-puzzle-place-congestion-openapi.json
  format: json
  label: SK Telecom Puzzle Place Congestion API
  slug: sk-telecom-puzzle-place-congestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-puzzle-place-congestion-openapi.json
- filename: sk-telecom-puzzle-residence-openapi.json
  format: json
  label: SK Telecom Puzzle Residence API
  slug: sk-telecom-puzzle-residence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-puzzle-residence-openapi.json
- filename: sk-telecom-meta-openapi.json
  format: json
  label: SK Telecom META API
  slug: sk-telecom-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-meta-openapi.json
- filename: sk-telecom-ovs-openapi.json
  format: json
  label: SK Telecom OVS API
  slug: sk-telecom-ovs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-ovs-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sk Telecom Authentication
name_suffix: Authentication
oauth_flows: []
overview: SK Telecom secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SK Telecom
provider_slug: sk-telecom
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: appKey
  sources:
  - openapi/sk-telecom-ax-tts-openapi.json
  - openapi/sk-telecom-facecan-openapi.json
  - openapi/sk-telecom-meta-openapi.json
  - openapi/sk-telecom-ovs-openapi.json
  type: apiKey
- in: header
  name: sec0
  parameter: appkey
  sources:
  - openapi/sk-telecom-puzzle-place-congestion-openapi.json
  - openapi/sk-telecom-puzzle-residence-openapi.json
  type: apiKey
slug: sk-telecom-authentication
source_filename: sk-telecom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: openapi/sk-telecom-ax-tts-openapi.json, openapi/sk-telecom-facecan-openapi.json, openapi/sk-telecom-meta-openapi.json,\n  openapi/sk-telecom-ovs-openapi.json, openapi/sk-telecom-puzzle-place-congestion-openapi.json,\n  openapi/sk-telecom-puzzle-residence-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: appKey\n  sources:\n  - openapi/sk-telecom-ax-tts-openapi.json\n  - openapi/sk-telecom-facecan-openapi.json\n  - openapi/sk-telecom-meta-openapi.json\n  - openapi/sk-telecom-ovs-openapi.json\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: appkey\n  sources:\n  - openapi/sk-telecom-puzzle-place-congestion-openapi.json\n  - openapi/sk-telecom-puzzle-residence-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/authentication/sk-telecom-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Telecommunications
- South Korea
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- 5G
- Identity Verification
- SIM Swap
- Artificial Intelligence
- Location
- Big Data
---
