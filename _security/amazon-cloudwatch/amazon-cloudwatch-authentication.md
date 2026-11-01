---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-cloudwatch-alarms-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Alarms API
  slug: amazon-cloudwatch-alarms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-alarms-api-openapi.yml
- filename: amazon-cloudwatch-dashboards-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Dashboards API
  slug: amazon-cloudwatch-dashboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-dashboards-api-openapi.yml
- filename: amazon-cloudwatch-metrics-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Metrics API
  slug: amazon-cloudwatch-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-metrics-api-openapi.yml
- filename: amazon-cloudwatch-amazon-cloudwatch-api-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Amazon CloudWatch API
  slug: amazon-cloudwatch-amazon-cloudwatch-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-amazon-cloudwatch-api-api-openapi.yml
- filename: amazon-cloudwatch-alarm-mute-rule-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Cloudwatch Alarm Mute Rule API
  slug: amazon-cloudwatch-alarm-mute-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-alarm-mute-rule-api-openapi.yml
- filename: amazon-cloudwatch-anomaly-detector-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Cloudwatch Anomaly Detector API
  slug: amazon-cloudwatch-anomaly-detector-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-anomaly-detector-api-openapi.yml
- filename: amazon-cloudwatch-insight-rule-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Cloudwatch Insight Rule API
  slug: amazon-cloudwatch-insight-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-insight-rule-api-openapi.yml
- filename: amazon-cloudwatch-metric-stream-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Cloudwatch Metric Stream API
  slug: amazon-cloudwatch-metric-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-metric-stream-api-openapi.yml
- filename: amazon-cloudwatch-o-tel-enrichment-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Cloudwatch O Tel Enrichment API
  slug: amazon-cloudwatch-o-tel-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-o-tel-enrichment-api-openapi.yml
- filename: amazon-cloudwatch-resource-metrics-configuration-api-openapi.yml
  format: yaml
  label: Amazon CloudWatch Cloudwatch Resource Metrics Configuration API
  slug: amazon-cloudwatch-resource-metrics-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudwatch/openapi/amazon-cloudwatch-resource-metrics-configuration-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/amazon-cloudwatch/authentication/amazon-cloudwatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
---
