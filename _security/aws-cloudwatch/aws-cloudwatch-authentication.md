---
api_key_in:
- header
api_specs:
- filename: aws-cloudwatch-openapi.yml
  format: yaml
  label: Amazon CloudWatch API
  slug: monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-cloudwatch/refs/heads/main/openapi/aws-cloudwatch-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Cloudwatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CloudWatch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CloudWatch
provider_slug: aws-cloudwatch
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-cloudwatch-openapi.yml
  type: apiKey
slug: aws-cloudwatch-authentication
source_filename: aws-cloudwatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-cloudwatch-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-cloudwatch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-cloudwatch/refs/heads/main/authentication/aws-cloudwatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Monitoring
- Observability
- Metrics
- Logs
- Alarms
- Cloud
---
