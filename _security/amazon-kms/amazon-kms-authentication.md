---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon KMS API
  slug: amazon-kms-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/kms/2014-11-01/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Kms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon KMS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon KMS
provider_slug: amazon-kms
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-kms-openapi.yml
  type: apiKey
slug: amazon-kms-authentication
source_filename: amazon-kms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-kms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-kms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kms/refs/heads/main/authentication/amazon-kms-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptography
- Data Protection
- Encryption
- Key Management
- Security
---
