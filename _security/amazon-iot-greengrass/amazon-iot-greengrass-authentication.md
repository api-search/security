---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-iot-greengrass-greengrass-api-openapi.yml
  format: yaml
  label: Amazon IoT Greengrass API
  slug: amazon-iot-greengrass-greengrass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iot-greengrass/openapi/amazon-iot-greengrass-greengrass-api-openapi.yml
- filename: amazon-iot-greengrass-tags-api-openapi.yml
  format: yaml
  label: Amazon IoT Greengrass Tags API
  slug: amazon-iot-greengrass-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iot-greengrass/openapi/amazon-iot-greengrass-tags-api-openapi.yml
- filename: amazon-iot-greengrass-certificateauthorities-api-openapi.yml
  format: yaml
  label: Amazon IoT Greengrass Iot Greengrass Certificateauthorities API
  slug: amazon-iot-greengrass-certificateauthorities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iot-greengrass/openapi/amazon-iot-greengrass-certificateauthorities-api-openapi.yml
- filename: amazon-iot-greengrass-operations-api-openapi.yml
  format: yaml
  label: Amazon IoT Greengrass Iot Greengrass Operations API
  slug: amazon-iot-greengrass-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iot-greengrass/openapi/amazon-iot-greengrass-operations-api-openapi.yml
- filename: amazon-iot-greengrass-role-api-openapi.yml
  format: yaml
  label: Amazon IoT Greengrass Iot Greengrass Role API
  slug: amazon-iot-greengrass-role-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iot-greengrass/openapi/amazon-iot-greengrass-role-api-openapi.yml
- filename: amazon-iot-greengrass-versions-api-openapi.yml
  format: yaml
  label: Amazon IoT Greengrass Iot Greengrass Versions API
  slug: amazon-iot-greengrass-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iot-greengrass/openapi/amazon-iot-greengrass-versions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon IoT Greengrass Authentication
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
source_yaml_url: https://artifacts.apis.io/amazon-iot-greengrass/authentication/amazon-iot-greengrass-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
---
