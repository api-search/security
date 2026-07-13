---
api_key_in:
- header
api_specs:
- filename: fonoa-validate-openapi.yml
  format: yaml
  label: Fonoa Validate API
  slug: validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-validate-openapi.yml
- filename: fonoa-tax-engine-openapi.yml
  format: yaml
  label: Fonoa Tax Engine API
  slug: tax-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-tax-engine-openapi.yml
- filename: fonoa-e-invoicing-openapi.yml
  format: yaml
  label: Fonoa E-Invoicing API
  slug: e-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-e-invoicing-openapi.yml
- filename: fonoa-onboarding-openapi.yml
  format: yaml
  label: Fonoa Onboarding API
  slug: onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-onboarding-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fonoa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fonoa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fonoa
provider_slug: fonoa
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/fonoa-e-invoicing-openapi.yml
  - openapi/fonoa-onboarding-openapi.yml
  - openapi/fonoa-tax-engine-openapi.yml
  - openapi/fonoa-validate-openapi.yml
  type: apiKey
slug: fonoa-authentication
source_filename: fonoa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fonoa-e-invoicing-openapi.yml, openapi/fonoa-onboarding-openapi.yml, openapi/fonoa-tax-engine-openapi.yml,\n  openapi/fonoa-validate-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/fonoa-e-invoicing-openapi.yml\n  - openapi/fonoa-onboarding-openapi.yml\n  - openapi/fonoa-tax-engine-openapi.yml\n  - openapi/fonoa-validate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/authentication/fonoa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Tax
- VAT
- GST
- E-Invoicing
- Tax Automation
- Tax Compliance
- Tax Calculation
- Tax ID Validation
- Invoice Generation
- Global Tax
- Indirect Tax
- FinTech
---
