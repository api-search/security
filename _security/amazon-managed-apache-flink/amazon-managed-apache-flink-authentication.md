---
api_key_in:
- header
api_specs:
- filename: amazon-managed-apache-flink-openapi-original.yaml
  format: yaml
  label: Amazon Managed Service for Apache Flink API
  slug: aws-managed-flink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/openapi/amazon-managed-apache-flink-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Managed Apache Flink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Managed Service for Apache Flink secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-managed-apache-flink-openapi-original.yaml
  type: apiKey
slug: amazon-managed-apache-flink-authentication
source_filename: amazon-managed-apache-flink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-managed-apache-flink-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-managed-apache-flink-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/authentication/amazon-managed-apache-flink-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
---
