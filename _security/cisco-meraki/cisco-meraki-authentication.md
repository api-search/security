---
api_key_in:
- header
api_specs:
- filename: cisco-meraki-appliance-api-openapi.yml
  format: yaml
  label: Cisco Meraki Appliance API
  slug: cisco-meraki-appliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-appliance-api-openapi.yml
- filename: cisco-meraki-camera-api-openapi.yml
  format: yaml
  label: Cisco Meraki Camera API
  slug: cisco-meraki-camera-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-camera-api-openapi.yml
- filename: cisco-meraki-devices-api-openapi.yml
  format: yaml
  label: Cisco Meraki Devices API
  slug: cisco-meraki-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-devices-api-openapi.yml
- filename: cisco-meraki-livetools-api-openapi.yml
  format: yaml
  label: Cisco Meraki LiveTools API
  slug: cisco-meraki-livetools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-livetools-api-openapi.yml
- filename: cisco-meraki-networks-api-openapi.yml
  format: yaml
  label: Cisco Meraki Networks API
  slug: cisco-meraki-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-networks-api-openapi.yml
- filename: cisco-meraki-organizations-api-openapi.yml
  format: yaml
  label: Cisco Meraki Organizations API
  slug: cisco-meraki-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-organizations-api-openapi.yml
- filename: cisco-meraki-switch-api-openapi.yml
  format: yaml
  label: Cisco Meraki Switch API
  slug: cisco-meraki-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-switch-api-openapi.yml
- filename: cisco-meraki-wireless-api-openapi.yml
  format: yaml
  label: Cisco Meraki Wireless API
  slug: cisco-meraki-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-wireless-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Meraki Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Meraki secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cisco Meraki
provider_slug: cisco-meraki
scheme_count: 2
schemes:
- in: header
  name: merakiApiKey
  parameter: X-Cisco-Meraki-API-Key
  sources:
  - openapi/cisco-meraki-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-meraki-openapi.yml
  type: http
slug: cisco-meraki-authentication
source_filename: cisco-meraki-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-meraki-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: merakiApiKey\n  type: apiKey\n  in: header\n  parameter: X-Cisco-Meraki-API-Key\n  sources:\n  - openapi/cisco-meraki-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cisco-meraki-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/authentication/cisco-meraki-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Networking
- Wireless
- Switching
- Security Appliances
- Cloud-Managed Networking
- MDM
- Cameras
- IoT
---
