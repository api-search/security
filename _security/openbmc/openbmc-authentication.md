---
api_key_in:
- header
api_specs:
- filename: openbmc-accountservice-api-openapi.yml
  format: yaml
  label: OpenBMC AccountService API
  slug: openbmc-accountservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-accountservice-api-openapi.yml
- filename: openbmc-chassis-api-openapi.yml
  format: yaml
  label: OpenBMC Chassis API
  slug: openbmc-chassis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-chassis-api-openapi.yml
- filename: openbmc-eventservice-api-openapi.yml
  format: yaml
  label: OpenBMC EventService API
  slug: openbmc-eventservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-eventservice-api-openapi.yml
- filename: openbmc-managers-api-openapi.yml
  format: yaml
  label: OpenBMC Managers API
  slug: openbmc-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-managers-api-openapi.yml
- filename: openbmc-openbmc-redfish-api-api-openapi.yml
  format: yaml
  label: OpenBMC OpenBMC Redfish API API
  slug: openbmc-openbmc-redfish-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-openbmc-redfish-api-api-openapi.yml
- filename: openbmc-sessionservice-api-openapi.yml
  format: yaml
  label: OpenBMC SessionService API
  slug: openbmc-sessionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-sessionservice-api-openapi.yml
- filename: openbmc-systems-api-openapi.yml
  format: yaml
  label: OpenBMC Systems API
  slug: openbmc-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-systems-api-openapi.yml
- filename: openbmc-updateservice-api-openapi.yml
  format: yaml
  label: OpenBMC UpdateService API
  slug: openbmc-updateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-updateservice-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openbmc Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenBMC secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenBMC
provider_slug: openbmc
scheme_count: 1
schemes:
- description: Redfish session token obtained from POST /SessionService/Sessions
  in: header
  name: SessionToken
  parameter: X-Auth-Token
  sources:
  - openapi/openbmc-openapi.yml
  type: apiKey
slug: openbmc-authentication
source_filename: openbmc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openbmc-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SessionToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Redfish session token obtained from POST /SessionService/Sessions\n  sources:\n  - openapi/openbmc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/authentication/openbmc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Firmware
- Hardware
- Linux Foundation
- Server
---
