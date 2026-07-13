---
api_key_in:
- header
api_specs:
- filename: amazon-iot-sitewise-openapi-original.yml
  format: yaml
  label: AWS IoT SiteWise API
  slug: aws-iot-sitewise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iot Sitewise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IoT SiteWise secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-iot-sitewise-openapi-original.yml
  type: apiKey
slug: amazon-iot-sitewise-authentication
source_filename: amazon-iot-sitewise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iot-sitewise-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-iot-sitewise-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/authentication/amazon-iot-sitewise-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
---
