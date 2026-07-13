---
api_key_in:
- header
api_specs:
- filename: amazon-payment-cryptography-openapi.yml
  format: yaml
  label: AWS Payment Cryptography API
  slug: aws-payment-cryptography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/openapi/amazon-payment-cryptography-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Payment Cryptography Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Payment Cryptography secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-payment-cryptography-openapi.yml
  type: apiKey
slug: amazon-payment-cryptography-authentication
source_filename: amazon-payment-cryptography-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-payment-cryptography-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-payment-cryptography-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/authentication/amazon-payment-cryptography-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
---
