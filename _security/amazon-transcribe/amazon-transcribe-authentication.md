---
api_key_in:
- header
api_specs:
- filename: amazon-transcribe-openapi.yml
  format: yaml
  label: Amazon Transcribe REST API
  slug: amazon-transcribe-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-transcribe/refs/heads/main/openapi/amazon-transcribe-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Transcribe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Transcribe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Transcribe
provider_slug: amazon-transcribe
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sig_v4
  parameter: Authorization
  sources:
  - openapi/amazon-transcribe-openapi.yml
  type: apiKey
slug: amazon-transcribe-authentication
source_filename: amazon-transcribe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-transcribe-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sig_v4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-transcribe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-transcribe/refs/heads/main/authentication/amazon-transcribe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Audio Processing
- Machine Learning
- Speech Recognition
- Speech-To-Text
- Transcription
---
