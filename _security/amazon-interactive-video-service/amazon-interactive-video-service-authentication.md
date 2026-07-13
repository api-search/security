---
api_key_in:
- header
api_specs:
- filename: amazon-ivs-openapi-original.yml
  format: yaml
  label: AWS Amazon IVS API
  slug: aws-ivs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/openapi/amazon-ivs-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Interactive Video Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Interactive Video Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-ivs-openapi-original.yml
  type: apiKey
slug: amazon-interactive-video-service-authentication
source_filename: amazon-interactive-video-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ivs-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-ivs-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/authentication/amazon-interactive-video-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Live Streaming
- Media
- Video
- Real-Time
---
