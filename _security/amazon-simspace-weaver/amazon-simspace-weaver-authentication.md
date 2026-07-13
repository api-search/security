---
api_key_in:
- header
api_specs:
- filename: amazon-simspace-weaver.yaml
  format: yaml
  label: AWS SimSpace Weaver API
  slug: aws-simspace-weaver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Simspace Weaver Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon SimSpace Weaver secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-simspace-weaver.yaml
  type: apiKey
slug: amazon-simspace-weaver-authentication
source_filename: amazon-simspace-weaver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-simspace-weaver.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-simspace-weaver.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/authentication/amazon-simspace-weaver-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
---
