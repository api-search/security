---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: emerson-electric-device-summary-api-openapi.yml
  format: yaml
  label: Emerson Electric Device Summary API
  slug: emerson-electric-device-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerson-electric/refs/heads/main/openapi/emerson-electric-device-summary-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Emerson Electric Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emerson Electric secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Emerson Electric
provider_slug: emerson-electric
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/emerson-electric-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/emerson-electric-openapi.yml
  type: apiKey
slug: emerson-electric-authentication
source_filename: emerson-electric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/emerson-electric-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/emerson-electric-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/emerson-electric-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerson-electric/refs/heads/main/authentication/emerson-electric-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Fortune 500
- Automation
- Industrial
- Process Control
- Measurement Instrumentation
- Devices
- APIs
---
