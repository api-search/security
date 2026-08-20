---
api_key_in:
- header
api_specs:
- filename: cloudwatch-alarms-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Alarms API
  slug: cloudwatch-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-alarms-api-openapi.yml
- filename: cloudwatch-anomaly-detection-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Anomaly Detection API
  slug: cloudwatch-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-anomaly-detection-api-openapi.yml
- filename: cloudwatch-composite-alarms-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Composite Alarms API
  slug: cloudwatch-composite-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-composite-alarms-api-openapi.yml
- filename: cloudwatch-dashboards-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Dashboards API
  slug: cloudwatch-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-dashboards-api-openapi.yml
- filename: cloudwatch-metric-streams-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Metric Streams API
  slug: cloudwatch-metric-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-metric-streams-api-openapi.yml
- filename: cloudwatch-metrics-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Metrics API
  slug: cloudwatch-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-metrics-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudwatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS CloudWatch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS CloudWatch
provider_slug: cloudwatch
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/cloudwatch-openapi.yml
  type: apiKey
slug: cloudwatch-authentication
source_filename: cloudwatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudwatch-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/cloudwatch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/authentication/cloudwatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alarms
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
---
