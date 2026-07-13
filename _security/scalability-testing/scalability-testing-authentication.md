---
api_key_in:
- header
api_specs:
- filename: loadtestservice.json
  format: json
  label: Azure Load Testing API
  slug: azure-load-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/loadtestservice/resource-manager/Microsoft.LoadTestService/stable/2022-12-01/loadtestservice.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scalability Testing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalability Testing secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Scalability Testing
provider_slug: scalability-testing
scheme_count: 2
schemes:
- bearerFormat: GrafanaToken
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/scalability-testing-openapi.yml
  type: http
- in: header
  name: StackId
  parameter: X-Stack-Id
  sources:
  - openapi/scalability-testing-openapi.yml
  type: apiKey
slug: scalability-testing-authentication
source_filename: scalability-testing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalability-testing-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: GrafanaToken\n  sources:\n  - openapi/scalability-testing-openapi.yml\n- name: StackId\n  type: apiKey\n  in: header\n  parameter: X-Stack-Id\n  sources:\n  - openapi/scalability-testing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalability-testing/refs/heads/main/authentication/scalability-testing-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- API Testing
- Load Testing
- Performance Testing
- Scalability
- Stress Testing
---
