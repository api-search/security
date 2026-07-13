---
api_key_in:
- header
api_specs:
- filename: amazon-healthlake-openapi.yaml
  format: yaml
  label: Amazon HealthLake API
  slug: amazon-healthlake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/openapi/amazon-healthlake-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Healthlake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon HealthLake secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-healthlake-openapi.yaml
  type: apiKey
slug: amazon-healthlake-authentication
source_filename: amazon-healthlake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-healthlake-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-healthlake-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/authentication/amazon-healthlake-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
---
