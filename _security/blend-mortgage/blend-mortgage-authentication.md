---
api_key_in: []
api_specs:
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Home Lending Applications API
  slug: blend-mortgage-home-lending-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Borrowers & Parties API
  slug: blend-mortgage-borrowers-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Documents & Disclosures API
  slug: blend-mortgage-documents-disclosures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Products & Pricing API
  slug: blend-mortgage-products-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Closings & eSignature API
  slug: blend-mortgage-closings-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Follow-ups (Tasks) API
  slug: blend-mortgage-follow-ups-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Events & Webhooks API
  slug: blend-mortgage-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Consumer Lending & Deposit Accounts API
  slug: blend-mortgage-consumer-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Lenders & Assignments API
  slug: blend-mortgage-lenders-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Reporting API
  slug: blend-mortgage-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Blend Mortgage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blend
provider_slug: blend-mortgage
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Blend authenticates requests with an authorization Bearer token. Each call must also send blend-api-version (to pin the API version) and blend-target-instance (tenant~instance) headers. API Secret Keys are exchanged for short-lived, request-scoped JWTs at Blend's API Gateway. Credentials are issued to Blend customers and certified partners - contact your Blend account team or partnerships to obtai
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blend-mortgage-openapi.yml
  type: http
slug: blend-mortgage-authentication
source_filename: blend-mortgage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blend-mortgage-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Blend authenticates requests with an authorization Bearer token. Each call must\n    also send blend-api-version (to pin the API version) and blend-target-instance (tenant~instance)\n    headers. API Secret Keys are exchanged for short-lived, request-scoped JWTs at Blend's API\n    Gateway. Credentials are issued to Blend customers and certified partners - contact your\n    Blend account team or partnerships to obtai\n  sources:\n  - openapi/blend-mortgage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/authentication/blend-mortgage-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Lending
- Mortgage
- Consumer Lending
- Account Opening
- FinTech
- Loan Origination
- Banking
- Financial Services
---
