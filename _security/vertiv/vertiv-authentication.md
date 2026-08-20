---
api_key_in:
- header
api_specs:
- filename: vertiv-alarms-api-openapi.yml
  format: yaml
  label: Vertiv Alarms API
  slug: vertiv-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-alarms-api-openapi.yml
- filename: vertiv-assets-api-openapi.yml
  format: yaml
  label: Vertiv Assets API
  slug: vertiv-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-assets-api-openapi.yml
- filename: vertiv-authentication-api-openapi.yml
  format: yaml
  label: Vertiv Authentication API
  slug: vertiv-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-authentication-api-openapi.yml
- filename: vertiv-circuits-api-openapi.yml
  format: yaml
  label: Vertiv Circuits API
  slug: vertiv-circuits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-circuits-api-openapi.yml
- filename: vertiv-data-sets-api-openapi.yml
  format: yaml
  label: Vertiv Data Sets API
  slug: vertiv-data-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-data-sets-api-openapi.yml
- filename: vertiv-devices-api-openapi.yml
  format: yaml
  label: Vertiv Devices API
  slug: vertiv-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-devices-api-openapi.yml
- filename: vertiv-racks-api-openapi.yml
  format: yaml
  label: Vertiv Racks API
  slug: vertiv-racks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-racks-api-openapi.yml
- filename: vertiv-sensors-api-openapi.yml
  format: yaml
  label: Vertiv Sensors API
  slug: vertiv-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-sensors-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vertiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vertiv secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vertiv
provider_slug: vertiv
scheme_count: 1
schemes:
- description: Session token obtained from the /auth endpoint
  in: header
  name: sessionToken
  parameter: X-Auth-Token
  sources:
  - openapi/vertiv-environet-alert-openapi.yml
  type: apiKey
slug: vertiv-authentication
source_filename: vertiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vertiv-environet-alert-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Session token obtained from the /auth endpoint\n  sources:\n  - openapi/vertiv-environet-alert-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/authentication/vertiv-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Critical Infrastructure
- Data-Center
- DCIM
- Infrastructure Monitoring
- Power Management
- UPS
---
