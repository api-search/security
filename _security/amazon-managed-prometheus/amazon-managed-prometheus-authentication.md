---
api_key_in:
- header
api_specs:
- filename: amazon-managed-prometheus-openapi-original.yaml
  format: yaml
  label: Amazon Managed Service for Prometheus API
  slug: amazon-managed-prometheus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/openapi/amazon-managed-prometheus-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Managed Prometheus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Managed Service for Prometheus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-managed-prometheus-openapi-original.yaml
  type: apiKey
slug: amazon-managed-prometheus-authentication
source_filename: amazon-managed-prometheus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-managed-prometheus-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-managed-prometheus-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/authentication/amazon-managed-prometheus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Containers
- Monitoring
- Observability
- Prometheus
---
