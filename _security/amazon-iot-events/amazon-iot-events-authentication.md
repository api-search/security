---
api_key_in:
- header
api_specs:
- filename: amazon-iot-events-alarm-models-api-openapi.yml
  format: yaml
  label: Amazon IoT Events Alarm Models API
  slug: amazon-iot-events-alarm-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/openapi/amazon-iot-events-alarm-models-api-openapi.yml
- filename: amazon-iot-events-analysis-api-openapi.yml
  format: yaml
  label: Amazon IoT Events Analysis API
  slug: amazon-iot-events-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/openapi/amazon-iot-events-analysis-api-openapi.yml
- filename: amazon-iot-events-detector-models-api-openapi.yml
  format: yaml
  label: Amazon IoT Events Detector Models API
  slug: amazon-iot-events-detector-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/openapi/amazon-iot-events-detector-models-api-openapi.yml
- filename: amazon-iot-events-input-routings-api-openapi.yml
  format: yaml
  label: Amazon IoT Events Input Routings API
  slug: amazon-iot-events-input-routings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/openapi/amazon-iot-events-input-routings-api-openapi.yml
- filename: amazon-iot-events-inputs-api-openapi.yml
  format: yaml
  label: Amazon IoT Events Inputs API
  slug: amazon-iot-events-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/openapi/amazon-iot-events-inputs-api-openapi.yml
- filename: amazon-iot-events-logging-api-openapi.yml
  format: yaml
  label: Amazon IoT Events Logging API
  slug: amazon-iot-events-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/openapi/amazon-iot-events-logging-api-openapi.yml
- filename: amazon-iot-events-tags-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon IoT Events Tags#resourceArn API
  slug: amazon-iot-events-tags-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/openapi/amazon-iot-events-tags-resourcearn-api-openapi.yml
- filename: amazon-iot-events-tags-resourcearn-tagkeys-api-openapi.yml
  format: yaml
  label: Amazon IoT Events Tags#resourceArn&tagKeys API
  slug: amazon-iot-events-tags-resourcearn-tagkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/openapi/amazon-iot-events-tags-resourcearn-tagkeys-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iot Events Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IoT Events secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-iot-events-openapi-original.yml
  type: apiKey
slug: amazon-iot-events-authentication
source_filename: amazon-iot-events-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iot-events-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-iot-events-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/authentication/amazon-iot-events-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Event Detection
- IoT
- State Machine
- Automation
---
