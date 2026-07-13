---
api_key_in:
- header
api_specs:
- filename: amazon-elastic-transcoder-openapi.yml
  format: yaml
  label: Amazon Elastic Transcoder API
  slug: amazon-elastic-transcoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/openapi/amazon-elastic-transcoder-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Elastic Transcoder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Elastic Transcoder secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-elastic-transcoder-openapi.yml
  type: apiKey
slug: amazon-elastic-transcoder-authentication
source_filename: amazon-elastic-transcoder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-elastic-transcoder-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-elastic-transcoder-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/authentication/amazon-elastic-transcoder-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
---
