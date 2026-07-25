---
api_key_in: []
api_specs:
- filename: idenfy-fraud-api-openapi.yml
  format: yaml
  label: iDenfy Fraud Prevention API
  slug: idenfy-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-fraud-api-openapi.yml
- filename: idenfy-face-authentication-api-openapi.yml
  format: yaml
  label: iDenfy Face Authentication API
  slug: idenfy-face-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-face-authentication-api-openapi.yml
- filename: idenfy-aml-api-openapi.yml
  format: yaml
  label: iDenfy Aml API
  slug: idenfy-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-aml-api-openapi.yml
- filename: idenfy-bank-api-openapi.yml
  format: yaml
  label: iDenfy Bank API
  slug: idenfy-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-bank-api-openapi.yml
- filename: idenfy-face-authentication-api-openapi.yml
  format: yaml
  label: iDenfy Face Authentication API
  slug: idenfy-face-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-face-authentication-api-openapi.yml
- filename: idenfy-fraud-api-openapi.yml
  format: yaml
  label: iDenfy Fraud API
  slug: idenfy-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-fraud-api-openapi.yml
- filename: idenfy-kyb-api-openapi.yml
  format: yaml
  label: iDenfy Kyb API
  slug: idenfy-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-kyb-api-openapi.yml
- filename: idenfy-kyc-api-openapi.yml
  format: yaml
  label: iDenfy Kyc API
  slug: idenfy-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-kyc-api-openapi.yml
- filename: idenfy-token-api-openapi.yml
  format: yaml
  label: iDenfy Token API
  slug: idenfy-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/openapi/idenfy-token-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Idenfy Authentication
name_suffix: Authentication
oauth_flows: []
overview: iDenfy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iDenfy
provider_slug: idenfy
scheme_count: 1
schemes:
- description: HTTP Basic auth using API_KEY as username and API_SECRET as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/idenfy-openapi.yml
  type: http
slug: idenfy-authentication
source_filename: idenfy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/idenfy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using API_KEY as username and API_SECRET as password.\n  sources:\n  - openapi/idenfy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idenfy/refs/heads/main/authentication/idenfy-authentication.yml
summary_line: http · 1 scheme
tags:
- AML
- Compliance
- Fraud Detection
- Identity Verification
- KYB
- KYC
---
