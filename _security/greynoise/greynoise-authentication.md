---
api_key_in:
- header
api_specs:
- filename: greynoise-openapi.yml
  format: yaml
  label: GreyNoise API
  slug: greynoise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Greynoise Authentication
name_suffix: Authentication
oauth_flows: []
overview: GreyNoise Intelligence secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GreyNoise Intelligence
provider_slug: greynoise
scheme_count: 1
schemes:
- description: GreyNoise API key passed via the 'key' HTTP header.
  in: header
  name: APIKeyHeaderAuth
  parameter: key
  sources:
  - openapi/greynoise-openapi.yml
  type: apiKey
slug: greynoise-authentication
source_filename: greynoise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/greynoise-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeaderAuth\n  type: apiKey\n  in: header\n  parameter: key\n  description: GreyNoise API key passed via the 'key' HTTP header.\n  sources:\n  - openapi/greynoise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/authentication/greynoise-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Threat Intelligence
- Cybersecurity
- IP Reputation
- Vulnerability Management
- Network Telemetry
- SOC Automation
- Public APIs
---
