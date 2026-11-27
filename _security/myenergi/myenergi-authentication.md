---
anonymous_access: false
api_key_in: []
api_specs:
- filename: myenergi-command-api-openapi.yml
  format: yaml
  label: myenergi Command API
  slug: myenergi-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-command-api-openapi.yml
- filename: myenergi-device-api-openapi.yml
  format: yaml
  label: myenergi Device API
  slug: myenergi-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-device-api-openapi.yml
- filename: myenergi-device-settings-api-openapi.yml
  format: yaml
  label: myenergi Device settings API
  slug: myenergi-device-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-device-settings-api-openapi.yml
- filename: myenergi-devices-api-openapi.yml
  format: yaml
  label: myenergi Devices API
  slug: myenergi-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-devices-api-openapi.yml
- filename: myenergi-gridpay-api-openapi.yml
  format: yaml
  label: myenergi Grid Pay API
  slug: myenergi-gridpay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-gridpay-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: myenergi Authentication
name_suffix: Authentication
oauth_flows: []
overview: myenergi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: myenergi
provider_slug: myenergi
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: API key generated on the myaccount website
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/myenergi-openapi.json
  type: http
slug: myenergi-authentication
source_filename: myenergi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/myenergi-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: API key generated on the myaccount website\n  sources:\n  - openapi/myenergi-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/myenergi/authentication/myenergi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Renewable Energy
- EV Charging
- Solar
- Battery Storage
---
