---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cisco-hardware-devices-api-openapi.yml
  format: yaml
  label: Cisco Hardware Devices API
  slug: cisco-hardware-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-devices-api-openapi.yml
- filename: cisco-hardware-administered-api-openapi.yml
  format: yaml
  label: Cisco Hardware Administered API
  slug: cisco-hardware-administered-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-administered-api-openapi.yml
- filename: cisco-hardware-appliance-api-openapi.yml
  format: yaml
  label: Cisco Hardware Appliance API
  slug: cisco-hardware-appliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-appliance-api-openapi.yml
- filename: cisco-hardware-camera-api-openapi.yml
  format: yaml
  label: Cisco Hardware Camera API
  slug: cisco-hardware-camera-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-camera-api-openapi.yml
- filename: cisco-hardware-campusgateway-api-openapi.yml
  format: yaml
  label: Cisco Hardware Campus Gateway API
  slug: cisco-hardware-campusgateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-campusgateway-api-openapi.yml
- filename: cisco-hardware-cellulargateway-api-openapi.yml
  format: yaml
  label: Cisco Hardware Cellular Gateway API
  slug: cisco-hardware-cellulargateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-cellulargateway-api-openapi.yml
- filename: cisco-hardware-insight-api-openapi.yml
  format: yaml
  label: Cisco Hardware Insight API
  slug: cisco-hardware-insight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-insight-api-openapi.yml
- filename: cisco-hardware-licensing-api-openapi.yml
  format: yaml
  label: Cisco Hardware Licensing API
  slug: cisco-hardware-licensing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-licensing-api-openapi.yml
- filename: cisco-hardware-networks-api-openapi.yml
  format: yaml
  label: Cisco Hardware Networks API
  slug: cisco-hardware-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-networks-api-openapi.yml
- filename: cisco-hardware-organizations-api-openapi.yml
  format: yaml
  label: Cisco Hardware Organizations API
  slug: cisco-hardware-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-organizations-api-openapi.yml
- filename: cisco-hardware-sensor-api-openapi.yml
  format: yaml
  label: Cisco Hardware Sensor API
  slug: cisco-hardware-sensor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-sensor-api-openapi.yml
- filename: cisco-hardware-sm-api-openapi.yml
  format: yaml
  label: Cisco Hardware Sm API
  slug: cisco-hardware-sm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-sm-api-openapi.yml
- filename: cisco-hardware-spaces-api-openapi.yml
  format: yaml
  label: Cisco Hardware Spaces API
  slug: cisco-hardware-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-spaces-api-openapi.yml
- filename: cisco-hardware-switch-api-openapi.yml
  format: yaml
  label: Cisco Hardware Switch API
  slug: cisco-hardware-switch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-switch-api-openapi.yml
- filename: cisco-hardware-wireless-api-openapi.yml
  format: yaml
  label: Cisco Hardware Wireless API
  slug: cisco-hardware-wireless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-wireless-api-openapi.yml
- filename: cisco-hardware-wirelesscontroller-api-openapi.yml
  format: yaml
  label: Cisco Hardware Wireless Controller API
  slug: cisco-hardware-wirelesscontroller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cisco-hardware/openapi/cisco-hardware-wirelesscontroller-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Cisco Hardware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Hardware secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cisco Hardware
provider_slug: cisco-hardware
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/cisco-hardware-openapi.yml
  type: http
- in: header
  name: tokenAuth
  parameter: X-Auth-Token
  sources:
  - openapi/cisco-hardware-openapi.yml
  type: apiKey
slug: cisco-hardware-authentication
source_filename: cisco-hardware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-hardware-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/cisco-hardware-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/cisco-hardware-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/cisco-hardware/authentication/cisco-hardware-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Hardware
- Infrastructure
- Networking
- Router
- Switches
---
