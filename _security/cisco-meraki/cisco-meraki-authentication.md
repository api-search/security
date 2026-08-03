---
api_key_in:
- header
api_specs:
- filename: cisco-meraki-administered-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Administered
  slug: administered
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-administered-api-openapi.json
- filename: cisco-meraki-appliance-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Appliance
  slug: appliance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-appliance-api-openapi.json
- filename: cisco-meraki-camera-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Camera
  slug: camera
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-camera-api-openapi.json
- filename: cisco-meraki-campusgateway-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — campusGateway
  slug: campusgateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-campusgateway-api-openapi.json
- filename: cisco-meraki-cellulargateway-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — cellularGateway
  slug: cellulargateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-cellulargateway-api-openapi.json
- filename: cisco-meraki-devices-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Devices
  slug: devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-devices-api-openapi.json
- filename: cisco-meraki-insight-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Insight
  slug: insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-insight-api-openapi.json
- filename: cisco-meraki-licensing-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Licensing
  slug: licensing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-licensing-api-openapi.json
- filename: cisco-meraki-networks-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Networks
  slug: networks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-networks-api-openapi.json
- filename: cisco-meraki-organizations-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Organizations
  slug: organizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-organizations-api-openapi.json
- filename: cisco-meraki-sensor-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Sensor
  slug: sensor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-sensor-api-openapi.json
- filename: cisco-meraki-sm-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Sm
  slug: sm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-sm-api-openapi.json
- filename: cisco-meraki-spaces-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Spaces
  slug: spaces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-spaces-api-openapi.json
- filename: cisco-meraki-switch-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Switch
  slug: switch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-switch-api-openapi.json
- filename: cisco-meraki-wireless-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — Wireless
  slug: wireless
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-wireless-api-openapi.json
- filename: cisco-meraki-wirelesscontroller-api-openapi.json
  format: json
  label: Cisco Meraki Dashboard API — wirelessController
  slug: wirelesscontroller
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-meraki/refs/heads/main/openapi/cisco-meraki-wirelesscontroller-api-openapi.json
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
  - openapi/cisco-meraki-dashboard-api-openapi.json (_original/)
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-meraki-dashboard-api-openapi.json (_original/)
  type: http
slug: cisco-meraki-authentication
source_filename: cisco-meraki-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-meraki-dashboard-api-openapi.json (_original/)\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: merakiApiKey\n  type: apiKey\n  in: header\n  parameter: X-Cisco-Meraki-API-Key\n  sources:\n  - openapi/cisco-meraki-dashboard-api-openapi.json (_original/)\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cisco-meraki-dashboard-api-openapi.json (_original/)\n"
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
