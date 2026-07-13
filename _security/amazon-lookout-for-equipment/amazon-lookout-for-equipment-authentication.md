---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Lookout for Equipment API
  slug: amazon-lookout-for-equipment-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/lookoutequipment/2020-12-15/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Lookout For Equipment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Lookout for Equipment secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Lookout for Equipment
provider_slug: amazon-lookout-for-equipment
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-lookout-for-equipment-openapi.yml
  type: apiKey
slug: amazon-lookout-for-equipment-authentication
source_filename: amazon-lookout-for-equipment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-lookout-for-equipment-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-lookout-for-equipment-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-equipment/refs/heads/main/authentication/amazon-lookout-for-equipment-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Equipment Monitoring
- Industrial IoT
- Machine Learning
- Predictive Maintenance
---
