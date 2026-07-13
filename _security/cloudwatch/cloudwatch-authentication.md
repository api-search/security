---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch API
  slug: amazon-cloudwatch-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/monitoring/2010-08-01/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Logs API
  slug: amazon-cloudwatch-logs-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/logs/2014-03-28/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Events API
  slug: amazon-cloudwatch-events-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/events/2015-10-07/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Application Insights API
  slug: amazon-cloudwatch-application-insights-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/application-insights/2018-11-25/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Synthetics API
  slug: amazon-cloudwatch-synthetics-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/synthetics/2017-10-11/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Internet Monitor API
  slug: amazon-cloudwatch-internet-monitor-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/internetmonitor/2021-06-03/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch RUM API
  slug: amazon-cloudwatch-rum-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/rum/2018-05-10/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Observability Access Manager API
  slug: amazon-cloudwatch-observability-access-manager-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/oam/2022-06-10/openapi.yaml
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
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
---
