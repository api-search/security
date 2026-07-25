---
api_key_in:
- header
api_specs:
- filename: brocade-communications-systems-chassis-api-openapi.yml
  format: yaml
  label: Brocade Communications Systems Chassis API
  slug: brocade-communications-systems-chassis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/openapi/brocade-communications-systems-chassis-api-openapi.yml
- filename: brocade-communications-systems-interfaces-api-openapi.yml
  format: yaml
  label: Brocade Communications Systems Interfaces API
  slug: brocade-communications-systems-interfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/openapi/brocade-communications-systems-interfaces-api-openapi.yml
- filename: brocade-communications-systems-operations-api-openapi.yml
  format: yaml
  label: Brocade Communications Systems Operations API
  slug: brocade-communications-systems-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/openapi/brocade-communications-systems-operations-api-openapi.yml
- filename: brocade-communications-systems-session-api-openapi.yml
  format: yaml
  label: Brocade Communications Systems Session API
  slug: brocade-communications-systems-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/openapi/brocade-communications-systems-session-api-openapi.yml
- filename: brocade-communications-systems-switch-api-openapi.yml
  format: yaml
  label: Brocade Communications Systems Switch API
  slug: brocade-communications-systems-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/openapi/brocade-communications-systems-switch-api-openapi.yml
- filename: brocade-communications-systems-zoning-api-openapi.yml
  format: yaml
  label: Brocade Communications Systems Zoning API
  slug: brocade-communications-systems-zoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/openapi/brocade-communications-systems-zoning-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Brocade Communications Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brocade Communications Systems secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Brocade Communications Systems
provider_slug: brocade-communications-systems
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/brocade-communications-systems-openapi.yml
  type: http
- in: header
  name: SessionToken
  parameter: Authorization
  sources:
  - openapi/brocade-communications-systems-openapi.yml
  type: apiKey
slug: brocade-communications-systems-authentication
source_filename: brocade-communications-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brocade-communications-systems-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/brocade-communications-systems-openapi.yml\n- name: SessionToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/brocade-communications-systems-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brocade-communications-systems/refs/heads/main/authentication/brocade-communications-systems-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data Networking
- Fibre Channel
- IP Networking
- Networking
- SAN
- Storage Networking
- Switches
- Fortune 1000
---
