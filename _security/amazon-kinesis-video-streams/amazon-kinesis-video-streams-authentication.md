---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Kinesis Video Streams API
  slug: amazon-kinesis-video-streams-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kinesisvideo/2017-09-30/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Kinesis Video Streams Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Kinesis Video Streams secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Kinesis Video Streams
provider_slug: amazon-kinesis-video-streams
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-kinesis-video-streams-openapi.yml
  type: apiKey
slug: amazon-kinesis-video-streams-authentication
source_filename: amazon-kinesis-video-streams-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-kinesis-video-streams-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-kinesis-video-streams-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-video-streams/refs/heads/main/authentication/amazon-kinesis-video-streams-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- IoT
- Machine Learning
- Media
- Video Streaming
---
