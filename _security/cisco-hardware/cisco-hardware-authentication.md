---
api_key_in:
- header
api_specs:
- filename: cisco-hardware-authentication-api-openapi.yml
  format: yaml
  label: Cisco Hardware Authentication API
  slug: cisco-hardware-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-authentication-api-openapi.yml
- filename: cisco-hardware-commandrunner-api-openapi.yml
  format: yaml
  label: Cisco Hardware CommandRunner API
  slug: cisco-hardware-commandrunner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-commandrunner-api-openapi.yml
- filename: cisco-hardware-devices-api-openapi.yml
  format: yaml
  label: Cisco Hardware Devices API
  slug: cisco-hardware-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-devices-api-openapi.yml
- filename: cisco-hardware-discovery-api-openapi.yml
  format: yaml
  label: Cisco Hardware Discovery API
  slug: cisco-hardware-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-discovery-api-openapi.yml
- filename: cisco-hardware-network-api-openapi.yml
  format: yaml
  label: Cisco Hardware Network API
  slug: cisco-hardware-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-network-api-openapi.yml
- filename: cisco-hardware-sites-api-openapi.yml
  format: yaml
  label: Cisco Hardware Sites API
  slug: cisco-hardware-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-sites-api-openapi.yml
- filename: cisco-hardware-topology-api-openapi.yml
  format: yaml
  label: Cisco Hardware Topology API
  slug: cisco-hardware-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-topology-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/authentication/cisco-hardware-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Hardware
- Infrastructure
- Networking
- Routers
- Switches
---
