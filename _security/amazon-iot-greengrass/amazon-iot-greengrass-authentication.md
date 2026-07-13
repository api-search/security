---
api_key_in:
- header
api_specs:
- filename: amazon-iot-greengrass-openapi-original.yml
  format: yaml
  label: AWS IoT Greengrass API
  slug: aws-iot-greengrass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/openapi/amazon-iot-greengrass-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iot Greengrass Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IoT Greengrass secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-iot-greengrass-openapi-original.yml
  type: apiKey
slug: amazon-iot-greengrass-authentication
source_filename: amazon-iot-greengrass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iot-greengrass-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-iot-greengrass-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/authentication/amazon-iot-greengrass-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
---
