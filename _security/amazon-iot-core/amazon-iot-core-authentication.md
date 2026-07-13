---
api_key_in:
- header
api_specs:
- filename: amazon-iot-core-openapi-original.yml
  format: yaml
  label: AWS IoT Core API
  slug: aws-iot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/openapi/amazon-iot-core-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iot Core Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IoT Core secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-iot-core-openapi-original.yml
  - openapi/amazon-iot-core-openapi.yml
  type: apiKey
slug: amazon-iot-core-authentication
source_filename: amazon-iot-core-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iot-core-openapi-original.yml, openapi/amazon-iot-core-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-iot-core-openapi-original.yml\n  - openapi/amazon-iot-core-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/authentication/amazon-iot-core-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Device Management
- IoT
- MQTT
- Message Routing
---
