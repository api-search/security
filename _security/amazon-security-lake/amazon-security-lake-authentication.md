---
api_key_in:
- header
api_specs:
- filename: amazon-security-lake-openapi.yml
  format: yaml
  label: Amazon Security Lake API
  slug: amazon-security-lake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-security-lake/refs/heads/main/openapi/amazon-security-lake-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Security Lake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Security Lake secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Security Lake
provider_slug: amazon-security-lake
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: AWSSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-security-lake-openapi.yml
  type: apiKey
slug: amazon-security-lake-authentication
source_filename: amazon-security-lake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-security-lake-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AWSSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-security-lake-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-security-lake/refs/heads/main/authentication/amazon-security-lake-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Lake
- Security
- SIEM
- Threat Detection
---
