---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-payment-cryptography-payment-cryptography-control-plane-api-openapi.yml
  format: yaml
  label: Amazon Payment Cryptography Payment Cryptography Control Plane API
  slug: amazon-payment-cryptography-payment-cryptography-control-plane-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-cryptography/openapi/amazon-payment-cryptography-payment-cryptography-control-plane-api-openapi.yml
- filename: amazon-payment-cryptography-default-key-replication-region-api-openapi.yml
  format: yaml
  label: Amazon Payment Cryptography Payment Cryptography Default Key Replication Region API
  slug: amazon-payment-cryptography-default-key-replication-region-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-cryptography/openapi/amazon-payment-cryptography-default-key-replication-region-api-openapi.yml
- filename: amazon-payment-cryptography-operations-api-openapi.yml
  format: yaml
  label: Amazon Payment Cryptography Payment Cryptography Operations API
  slug: amazon-payment-cryptography-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-cryptography/openapi/amazon-payment-cryptography-operations-api-openapi.yml
- filename: amazon-payment-cryptography-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon Payment Cryptography Payment Cryptography Resource Policy API
  slug: amazon-payment-cryptography-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-cryptography/openapi/amazon-payment-cryptography-resource-policy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/amazon-payment-cryptography/authentication/amazon-payment-cryptography-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
---
