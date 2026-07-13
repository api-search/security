---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS Resilience Hub API
  slug: aws-resilience-hub-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/resiliencehub/2020-04-30/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Resilience Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Resilience Hub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Resilience Hub
provider_slug: amazon-resilience-hub
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_signature
  parameter: Authorization
  sources:
  - openapi/amazon-resilience-hub-openapi.yml
  type: apiKey
slug: amazon-resilience-hub-authentication
source_filename: amazon-resilience-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-resilience-hub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_signature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-resilience-hub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-resilience-hub/refs/heads/main/authentication/amazon-resilience-hub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Disaster Recovery
- High Availability
- Operations
- Resilience
---
