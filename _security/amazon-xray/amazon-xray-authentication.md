---
api_key_in:
- header
api_specs:
- filename: amazon-xray-openapi-original.yaml
  format: yaml
  label: Amazon X-Ray REST API
  slug: amazon-xray-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/openapi/amazon-xray-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Xray Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon X-Ray secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon X-Ray
provider_slug: amazon-xray
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-xray-openapi-original.yaml
  - openapi/amazon-xray-openapi.yml
  type: apiKey
slug: amazon-xray-authentication
source_filename: amazon-xray-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-xray-openapi-original.yaml, openapi/amazon-xray-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-xray-openapi-original.yaml\n  - openapi/amazon-xray-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/authentication/amazon-xray-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
---
