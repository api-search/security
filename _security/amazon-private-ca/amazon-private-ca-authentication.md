---
api_key_in:
- header
api_specs:
- filename: amazon-private-ca-openapi-original.yaml
  format: yaml
  label: AWS Private CA API
  slug: aws-private-ca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/openapi/amazon-private-ca-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Private Ca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Private CA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-private-ca-openapi-original.yaml
  type: apiKey
slug: amazon-private-ca-authentication
source_filename: amazon-private-ca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-private-ca-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-private-ca-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/authentication/amazon-private-ca-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
---
