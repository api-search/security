---
api_key_in:
- header
api_specs:
- filename: super-micro-computer-accounts-api-openapi.yml
  format: yaml
  label: Super Micro Computer Accounts API
  slug: super-micro-computer-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-accounts-api-openapi.yml
- filename: super-micro-computer-chassis-api-openapi.yml
  format: yaml
  label: Super Micro Computer Chassis API
  slug: super-micro-computer-chassis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-chassis-api-openapi.yml
- filename: super-micro-computer-event-service-api-openapi.yml
  format: yaml
  label: Super Micro Computer Event Service API
  slug: super-micro-computer-event-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-event-service-api-openapi.yml
- filename: super-micro-computer-managers-api-openapi.yml
  format: yaml
  label: Super Micro Computer Managers API
  slug: super-micro-computer-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-managers-api-openapi.yml
- filename: super-micro-computer-network-api-openapi.yml
  format: yaml
  label: Super Micro Computer Network API
  slug: super-micro-computer-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-network-api-openapi.yml
- filename: super-micro-computer-service-root-api-openapi.yml
  format: yaml
  label: Super Micro Computer Service Root API
  slug: super-micro-computer-service-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-service-root-api-openapi.yml
- filename: super-micro-computer-sessions-api-openapi.yml
  format: yaml
  label: Super Micro Computer Sessions API
  slug: super-micro-computer-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-sessions-api-openapi.yml
- filename: super-micro-computer-storage-api-openapi.yml
  format: yaml
  label: Super Micro Computer Storage API
  slug: super-micro-computer-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-storage-api-openapi.yml
- filename: super-micro-computer-systems-api-openapi.yml
  format: yaml
  label: Super Micro Computer Systems API
  slug: super-micro-computer-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-systems-api-openapi.yml
- filename: super-micro-computer-update-service-api-openapi.yml
  format: yaml
  label: Super Micro Computer Update Service API
  slug: super-micro-computer-update-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-micro-computer/refs/heads/main/openapi/super-micro-computer-update-service-api-openapi.yml
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
