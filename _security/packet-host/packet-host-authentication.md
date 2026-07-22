---
api_key_in:
- header
api_specs:
- filename: packet-host-metal-openapi-original.yml
  format: yaml
  label: Metal API
  slug: metal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packet-host/refs/heads/main/openapi/packet-host-metal-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Packet Host Authentication
name_suffix: Authentication
oauth_flows: []
overview: Packet Host secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Packet Host
provider_slug: packet-host
scheme_count: 1
schemes:
- description: HTTP header containing the User or Project API key that will be used to authenticate the request.
  in: header
  name: x_auth_token
  parameter: X-Auth-Token
  sources:
  - openapi/packet-host-metal-openapi-original.yml
  type: apiKey
slug: packet-host-authentication
source_filename: packet-host-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/packet-host-metal-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x_auth_token\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: HTTP header containing the User or Project API key that will be used to authenticate\n    the request.\n  sources:\n  - openapi/packet-host-metal-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packet-host/refs/heads/main/authentication/packet-host-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Bare Metal
- Cloud Infrastructure
- Infrastructure as a Service
- Servers
- Compute
- Provisioning
- Equinix Metal
- Retired
---
