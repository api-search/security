---
api_key_in:
- header
api_specs:
- filename: amazon-data-exchange-openapi.yml
  format: yaml
  label: AWS Data Exchange API
  slug: aws-data-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/openapi/amazon-data-exchange-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Data Exchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Data Exchange secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: awsSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-data-exchange-openapi.yml
  type: apiKey
slug: amazon-data-exchange-authentication
source_filename: amazon-data-exchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-data-exchange-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-data-exchange-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/authentication/amazon-data-exchange-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
---
