---
api_key_in: []
api_specs:
- filename: credilinqai-authentication-api-openapi.yml
  format: yaml
  label: Credilinq.ai Authentication API
  slug: credilinqai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-authentication-api-openapi.yml
- filename: credilinqai-customers-api-openapi.yml
  format: yaml
  label: Credilinq.ai Customers API
  slug: credilinqai-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-customers-api-openapi.yml
- filename: credilinqai-kyc-api-openapi.yml
  format: yaml
  label: Credilinq.ai KYC API
  slug: credilinqai-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-kyc-api-openapi.yml
- filename: credilinqai-loans-api-openapi.yml
  format: yaml
  label: Credilinq.ai Loans API
  slug: credilinqai-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-loans-api-openapi.yml
- filename: credilinqai-miscellaneous-api-openapi.yml
  format: yaml
  label: Credilinq.ai Miscellaneous API
  slug: credilinqai-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-miscellaneous-api-openapi.yml
- filename: credilinqai-onboarding-api-openapi.yml
  format: yaml
  label: Credilinq.ai Onboarding API
  slug: credilinqai-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-onboarding-api-openapi.yml
- filename: credilinqai-payment-api-openapi.yml
  format: yaml
  label: Credilinq.ai Payment API
  slug: credilinqai-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-payment-api-openapi.yml
- filename: credilinqai-report-api-openapi.yml
  format: yaml
  label: Credilinq.ai Report API
  slug: credilinqai-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-report-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Credilinqai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credilinq.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Credilinq.ai
provider_slug: credilinqai
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: access-token
  scheme: bearer
  sources:
  - openapi/credilinqai-openapi.yml
  type: http
slug: credilinqai-authentication
source_filename: credilinqai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/credilinqai-openapi.yml\ndocs: https://docs.credilinq.ai/docs/authentication-1.md\nsummary:\n  types:\n  - http\n  model: oauth2-client-credentials\n  notes: >-\n    CrediLinq uses Auth0 for authentication. Customers request client_id /\n    client_secret from the CrediLinq support team (issued per environment:\n    Sandbox, Staging, Production). The client POSTs those credentials to the\n    token endpoint to obtain a Bearer JWT access token (token_type \"Bearer\",\n    default TTL 8 hours), which is then sent in the Authorization header on all\n    subsequent requests. Tokens should be cached until expiry.\ntoken_endpoint: https://api.credilinq.ai/v1/auth/generate-token\ntoken_operation: AuthenticationController_generateToken\nschemes:\n- name: access-token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/credilinqai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/authentication/credilinqai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Embedded Finance
- Lending
- BNPL
- Credit
- Payments
- KYC
- B2B
---
