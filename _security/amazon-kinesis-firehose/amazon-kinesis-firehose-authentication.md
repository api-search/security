---
api_key_in:
- header
api_specs:
- filename: amazon-kinesis-firehose-openapi.yml
  format: yaml
  label: Amazon Kinesis Data Firehose API
  slug: amazon-kinesis-data-firehose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-firehose/refs/heads/main/openapi/amazon-kinesis-firehose-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Kinesis Firehose Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Kinesis Data Firehose secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Kinesis Data Firehose
provider_slug: amazon-kinesis-firehose
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-kinesis-firehose-openapi.yml
  type: apiKey
slug: amazon-kinesis-firehose-authentication
source_filename: amazon-kinesis-firehose-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-kinesis-firehose-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-kinesis-firehose-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-firehose/refs/heads/main/authentication/amazon-kinesis-firehose-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Data Delivery
- Streaming
---
