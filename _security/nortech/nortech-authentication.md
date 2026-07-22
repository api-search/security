---
api_key_in: []
api_specs:
- filename: nortech-openapi-original.json
  format: json
  label: Nortech Cloud API
  slug: nortech-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nortech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nortech secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nortech
provider_slug: nortech
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: Bearer Token
  scheme: bearer
  sources:
  - openapi/nortech-openapi-original.json
  type: http
slug: nortech-authentication
source_filename: nortech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nortech-openapi-original.json\ndocs: https://docs.apps.nor.tech/cloud-apis-sdks-http-api\nnotes: >-\n  HTTP Bearer (JWT) authentication. Tokens are provisioned on request from\n  support@nortech.ai. The same Bearer token is used as the MQTT broker password\n  for live-data streaming.\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nortech-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/authentication/nortech-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Industrial IoT
- IIoT
- Maritime
- Operational Data
- Time Series
- Sensors
- Data Infrastructure
---
