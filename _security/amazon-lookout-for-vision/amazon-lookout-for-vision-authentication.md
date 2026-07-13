---
api_key_in:
- header
api_specs:
- filename: amazon-lookout-for-vision-openapi-original.yaml
  format: yaml
  label: Amazon Lookout for Vision API
  slug: amazon-lookout-for-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/openapi/amazon-lookout-for-vision-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Lookout For Vision Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Lookout for Vision secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-lookout-for-vision-openapi-original.yaml
  type: apiKey
slug: amazon-lookout-for-vision-authentication
source_filename: amazon-lookout-for-vision-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-lookout-for-vision-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-lookout-for-vision-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/authentication/amazon-lookout-for-vision-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
---
