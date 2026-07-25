---
api_key_in:
- header
api_specs:
- filename: amazon-iot-twinmaker-pricingplan-api-openapi.yml
  format: yaml
  label: Amazon IoT TwinMaker Pricingplan API
  slug: amazon-iot-twinmaker-pricingplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/openapi/amazon-iot-twinmaker-pricingplan-api-openapi.yml
- filename: amazon-iot-twinmaker-queries-api-openapi.yml
  format: yaml
  label: Amazon IoT TwinMaker Queries API
  slug: amazon-iot-twinmaker-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/openapi/amazon-iot-twinmaker-queries-api-openapi.yml
- filename: amazon-iot-twinmaker-sync-jobs-api-openapi.yml
  format: yaml
  label: Amazon IoT TwinMaker Sync Jobs API
  slug: amazon-iot-twinmaker-sync-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/openapi/amazon-iot-twinmaker-sync-jobs-api-openapi.yml
- filename: amazon-iot-twinmaker-tags-api-openapi.yml
  format: yaml
  label: Amazon IoT TwinMaker Tags API
  slug: amazon-iot-twinmaker-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/openapi/amazon-iot-twinmaker-tags-api-openapi.yml
- filename: amazon-iot-twinmaker-tags-list-api-openapi.yml
  format: yaml
  label: Amazon IoT TwinMaker Tags List API
  slug: amazon-iot-twinmaker-tags-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/openapi/amazon-iot-twinmaker-tags-list-api-openapi.yml
- filename: amazon-iot-twinmaker-tags-resourcearn-tagkeys-api-openapi.yml
  format: yaml
  label: Amazon IoT TwinMaker Tags#resourceARN&tagKeys API
  slug: amazon-iot-twinmaker-tags-resourcearn-tagkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/openapi/amazon-iot-twinmaker-tags-resourcearn-tagkeys-api-openapi.yml
- filename: amazon-iot-twinmaker-workspaces-api-openapi.yml
  format: yaml
  label: Amazon IoT TwinMaker Workspaces API
  slug: amazon-iot-twinmaker-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/openapi/amazon-iot-twinmaker-workspaces-api-openapi.yml
- filename: amazon-iot-twinmaker-workspaces-list-api-openapi.yml
  format: yaml
  label: Amazon IoT TwinMaker Workspaces List API
  slug: amazon-iot-twinmaker-workspaces-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/openapi/amazon-iot-twinmaker-workspaces-list-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iot Twinmaker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IoT TwinMaker secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-iot-twinmaker-openapi-original.yml
  type: apiKey
slug: amazon-iot-twinmaker-authentication
source_filename: amazon-iot-twinmaker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iot-twinmaker-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-iot-twinmaker-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/authentication/amazon-iot-twinmaker-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
---
