---
api_key_in:
- header
api_specs:
- filename: amazon-cloudwatch-alarms-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Alarms API
  slug: amazon-cloudwatch-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/openapi/amazon-cloudwatch-alarms-api-openapi.yml
- filename: amazon-cloudwatch-dashboards-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Dashboards API
  slug: amazon-cloudwatch-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/openapi/amazon-cloudwatch-dashboards-api-openapi.yml
- filename: amazon-cloudwatch-metrics-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Metrics API
  slug: amazon-cloudwatch-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/openapi/amazon-cloudwatch-metrics-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Cloudwatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CloudWatch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4Auth
  parameter: Authorization
  sources:
  - openapi/amazon-cloudwatch-openapi.yml
  type: apiKey
slug: amazon-cloudwatch-authentication
source_filename: amazon-cloudwatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-cloudwatch-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-cloudwatch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/authentication/amazon-cloudwatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
---
