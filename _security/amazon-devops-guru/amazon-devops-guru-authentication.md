---
api_key_in:
- header
api_specs:
- filename: amazon-devops-guru-accounts-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Accounts API
  slug: amazon-devops-guru-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-accounts-api-openapi.yml
- filename: amazon-devops-guru-anomalies-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Anomalies API
  slug: amazon-devops-guru-anomalies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-anomalies-api-openapi.yml
- filename: amazon-devops-guru-channels-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Channels API
  slug: amazon-devops-guru-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-channels-api-openapi.yml
- filename: amazon-devops-guru-cost-estimation-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Cost Estimation API
  slug: amazon-devops-guru-cost-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-cost-estimation-api-openapi.yml
- filename: amazon-devops-guru-event-sources-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Event Sources API
  slug: amazon-devops-guru-event-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-event-sources-api-openapi.yml
- filename: amazon-devops-guru-events-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Events API
  slug: amazon-devops-guru-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-events-api-openapi.yml
- filename: amazon-devops-guru-feedback-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Feedback API
  slug: amazon-devops-guru-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-feedback-api-openapi.yml
- filename: amazon-devops-guru-insights-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Insights API
  slug: amazon-devops-guru-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-insights-api-openapi.yml
- filename: amazon-devops-guru-list-log-anomalies-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru List Log Anomalies API
  slug: amazon-devops-guru-list-log-anomalies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-list-log-anomalies-api-openapi.yml
- filename: amazon-devops-guru-monitoredresources-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru MonitoredResources API
  slug: amazon-devops-guru-monitoredresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-monitoredresources-api-openapi.yml
- filename: amazon-devops-guru-organization-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Organization API
  slug: amazon-devops-guru-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-organization-api-openapi.yml
- filename: amazon-devops-guru-recommendations-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Recommendations API
  slug: amazon-devops-guru-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-recommendations-api-openapi.yml
- filename: amazon-devops-guru-resource-collections-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Resource Collections API
  slug: amazon-devops-guru-resource-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-resource-collections-api-openapi.yml
- filename: amazon-devops-guru-service-integrations-api-openapi.yml
  format: yaml
  label: Amazon DevOps Guru Service Integrations API
  slug: amazon-devops-guru-service-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/openapi/amazon-devops-guru-service-integrations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Devops Guru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DevOps Guru secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-devops-guru-openapi.yaml
  type: apiKey
slug: amazon-devops-guru-authentication
source_filename: amazon-devops-guru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-devops-guru-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-devops-guru-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/authentication/amazon-devops-guru-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Anomaly Detection
- DevOps
- Machine-Learning
- Operational Intelligence
---
