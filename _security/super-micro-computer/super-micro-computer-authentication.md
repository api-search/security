---
api_key_in:
- header
api_specs:
- filename: supermicro-redfish-openapi.yml
  format: yaml
  label: Supermicro Redfish API
  slug: redfish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/supermicro-redfish-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Super Micro Computer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Super Micro Computer secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Super Micro Computer
provider_slug: super-micro-computer
scheme_count: 2
schemes:
- description: HTTP Basic authentication using BMC username and password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/supermicro-redfish-openapi.yml
  type: http
- description: Redfish session token obtained from POST /redfish/v1/SessionService/Sessions
  in: header
  name: SessionAuth
  parameter: X-Auth-Token
  sources:
  - openapi/supermicro-redfish-openapi.yml
  type: apiKey
slug: super-micro-computer-authentication
source_filename: super-micro-computer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/supermicro-redfish-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using BMC username and password\n  sources:\n  - openapi/supermicro-redfish-openapi.yml\n- name: SessionAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Redfish session token obtained from POST /redfish/v1/SessionService/Sessions\n  sources:\n  - openapi/supermicro-redfish-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/authentication/super-micro-computer-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Servers
- Data Center
- Hardware
- Server Management
- Redfish
- BMC
- IPMI
- Fortune 500
- Infrastructure
- Cloud
---
