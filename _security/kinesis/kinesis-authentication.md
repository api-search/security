---
api_key_in:
- header
api_specs:
- filename: amazon-kinesis-data-streams-openapi-original.yml
  format: yaml
  label: Amazon Kinesis Data Streams API
  slug: data-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/openapi/amazon-kinesis-data-streams-openapi-original.yml
- filename: amazon-data-firehose-openapi-original.yml
  format: yaml
  label: Amazon Data Firehose API
  slug: data-firehose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/openapi/amazon-data-firehose-openapi-original.yml
- filename: amazon-kinesis-data-analytics-openapi-original.yml
  format: yaml
  label: Amazon Kinesis Data Analytics API
  slug: data-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/openapi/amazon-kinesis-data-analytics-openapi-original.yml
- filename: amazon-kinesis-video-streams-openapi-original.yml
  format: yaml
  label: Amazon Kinesis Video Streams API
  slug: video-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/openapi/amazon-kinesis-video-streams-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kinesis Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Kinesis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Kinesis
provider_slug: kinesis
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-data-firehose-openapi-original.yml
  - openapi/amazon-kinesis-data-analytics-openapi-original.yml
  - openapi/amazon-kinesis-data-streams-openapi-original.yml
  - openapi/amazon-kinesis-video-streams-openapi-original.yml
  type: apiKey
slug: kinesis-authentication
source_filename: kinesis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-data-firehose-openapi-original.yml, openapi/amazon-kinesis-data-analytics-openapi-original.yml,\n  openapi/amazon-kinesis-data-streams-openapi-original.yml, openapi/amazon-kinesis-video-streams-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-data-firehose-openapi-original.yml\n  - openapi/amazon-kinesis-data-analytics-openapi-original.yml\n  - openapi/amazon-kinesis-data-streams-openapi-original.yml\n  - openapi/amazon-kinesis-video-streams-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinesis/refs/heads/main/authentication/kinesis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Apache Flink
- Big Data
- Data Processing
- Real-Time
- Streaming
- Video
---
