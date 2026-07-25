---
api_key_in:
- header
api_specs:
- filename: cisco-clients-api-openapi.yml
  format: yaml
  label: Cisco Clients API
  slug: cisco-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/openapi/cisco-clients-api-openapi.yml
- filename: cisco-devices-api-openapi.yml
  format: yaml
  label: Cisco Devices API
  slug: cisco-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/openapi/cisco-devices-api-openapi.yml
- filename: cisco-networks-api-openapi.yml
  format: yaml
  label: Cisco Networks API
  slug: cisco-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/openapi/cisco-networks-api-openapi.yml
- filename: cisco-organizations-api-openapi.yml
  format: yaml
  label: Cisco Organizations API
  slug: cisco-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/openapi/cisco-organizations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco
provider_slug: cisco
scheme_count: 1
schemes:
- description: Meraki Dashboard API key.
  in: header
  name: apiKeyAuth
  parameter: X-Cisco-Meraki-API-Key
  sources:
  - openapi/cisco-meraki-api.yaml
  type: apiKey
slug: cisco-authentication
source_filename: cisco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-meraki-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Cisco-Meraki-API-Key\n  description: Meraki Dashboard API key.\n  sources:\n  - openapi/cisco-meraki-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/authentication/cisco-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fortune 100
- Collaboration
- Enterprise
- Networking
- Security
- SD-WAN
---
