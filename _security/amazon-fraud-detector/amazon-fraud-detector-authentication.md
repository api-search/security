---
api_key_in:
- header
api_specs:
- filename: amazon-fraud-detector-openapi.yml
  format: yaml
  label: Amazon Fraud Detector API
  slug: amazon-fraud-detector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/openapi/amazon-fraud-detector-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Fraud Detector Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Fraud Detector secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Fraud Detector
provider_slug: amazon-fraud-detector
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: awsSigV4
  parameter: Authorization
  sources:
  - openapi/amazon-fraud-detector-openapi.yml
  type: apiKey
slug: amazon-fraud-detector-authentication
source_filename: amazon-fraud-detector-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-fraud-detector-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-fraud-detector-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/authentication/amazon-fraud-detector-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial Services
- Fraud Detection
- Machine Learning
- Security
---
