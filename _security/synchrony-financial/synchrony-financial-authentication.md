---
api_key_in: []
api_specs:
- filename: synchrony-financial-applications-api-openapi.yml
  format: yaml
  label: Synchrony Financial Applications API
  slug: synchrony-financial-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-applications-api-openapi.yml
- filename: synchrony-financial-decisions-api-openapi.yml
  format: yaml
  label: Synchrony Financial Decisions API
  slug: synchrony-financial-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-decisions-api-openapi.yml
- filename: synchrony-financial-payments-api-openapi.yml
  format: yaml
  label: Synchrony Financial Payments API
  slug: synchrony-financial-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-payments-api-openapi.yml
- filename: synchrony-financial-preapprovals-api-openapi.yml
  format: yaml
  label: Synchrony Financial Preapprovals API
  slug: synchrony-financial-preapprovals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-preapprovals-api-openapi.yml
- filename: synchrony-financial-preauthorizations-api-openapi.yml
  format: yaml
  label: Synchrony Financial Preauthorizations API
  slug: synchrony-financial-preauthorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-preauthorizations-api-openapi.yml
- filename: synchrony-financial-purchases-api-openapi.yml
  format: yaml
  label: Synchrony Financial Purchases API
  slug: synchrony-financial-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-purchases-api-openapi.yml
- filename: synchrony-financial-refunds-api-openapi.yml
  format: yaml
  label: Synchrony Financial Refunds API
  slug: synchrony-financial-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-refunds-api-openapi.yml
- filename: synchrony-financial-reversals-api-openapi.yml
  format: yaml
  label: Synchrony Financial Reversals API
  slug: synchrony-financial-reversals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-reversals-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Synchrony Financial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synchrony Financial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synchrony Financial
provider_slug: synchrony-financial
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/synchrony-financial-credit-authorization-openapi.yml
  - openapi/synchrony-financial-quickscreen-apply-openapi.yml
  type: http
slug: synchrony-financial-authentication
source_filename: synchrony-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synchrony-financial-credit-authorization-openapi.yml, openapi/synchrony-financial-quickscreen-apply-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/synchrony-financial-credit-authorization-openapi.yml\n  - openapi/synchrony-financial-quickscreen-apply-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/authentication/synchrony-financial-authentication.yml
summary_line: http · 1 scheme
tags:
- Financial-Services
- Credit
- Payments
- Consumer Finance
- Retail Finance
---
