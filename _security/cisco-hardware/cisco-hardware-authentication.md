---
api_key_in:
- header
api_specs:
- filename: openapiSpec
  format: yaml
  label: Cisco Meraki Dashboard API
  slug: meraki-dashboard-api
  spec_type: OpenAPI
  url: https://api.meraki.com/api/v1/openapiSpec
- filename: openapi.yaml
  format: yaml
  label: Cisco Intersight API
  slug: intersight-api
  spec_type: OpenAPI
  url: https://intersight.com/apidocs/downloads/
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
