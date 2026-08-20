---
api_key_in:
- header
api_specs:
- filename: sikoia-adverse-media-api-openapi.yml
  format: yaml
  label: Sikoia Adverse Media API
  slug: sikoia-adverse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-adverse-media-api-openapi.yml
- filename: sikoia-affordability-insights-api-openapi.yml
  format: yaml
  label: Sikoia Affordability Insights API
  slug: sikoia-affordability-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-affordability-insights-api-openapi.yml
- filename: sikoia-authentication-api-openapi.yml
  format: yaml
  label: Sikoia Authentication API
  slug: sikoia-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-authentication-api-openapi.yml
- filename: sikoia-banking-api-openapi.yml
  format: yaml
  label: Sikoia Banking API
  slug: sikoia-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-banking-api-openapi.yml
- filename: sikoia-cases-api-openapi.yml
  format: yaml
  label: Sikoia Cases API
  slug: sikoia-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-cases-api-openapi.yml
- filename: sikoia-checklist-api-openapi.yml
  format: yaml
  label: Sikoia Checklist API
  slug: sikoia-checklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-checklist-api-openapi.yml
- filename: sikoia-companies-people-api-openapi.yml
  format: yaml
  label: Sikoia Companies & People API
  slug: sikoia-companies-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-companies-people-api-openapi.yml
- filename: sikoia-company-credit-report-api-openapi.yml
  format: yaml
  label: Sikoia Company Credit Report API
  slug: sikoia-company-credit-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-company-credit-report-api-openapi.yml
- filename: sikoia-company-registry-api-openapi.yml
  format: yaml
  label: Sikoia Company Registry API
  slug: sikoia-company-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-company-registry-api-openapi.yml
- filename: sikoia-data-sources-api-openapi.yml
  format: yaml
  label: Sikoia Data Sources API
  slug: sikoia-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-data-sources-api-openapi.yml
- filename: sikoia-documents-api-openapi.yml
  format: yaml
  label: Sikoia Documents API
  slug: sikoia-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-documents-api-openapi.yml
- filename: sikoia-excel-report-api-openapi.yml
  format: yaml
  label: Sikoia Excel Report API
  slug: sikoia-excel-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-excel-report-api-openapi.yml
- filename: sikoia-identity-verification-api-openapi.yml
  format: yaml
  label: Sikoia Identity Verification API
  slug: sikoia-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-identity-verification-api-openapi.yml
- filename: sikoia-income-employer-verification-api-openapi.yml
  format: yaml
  label: Sikoia Income & Employer Verification API
  slug: sikoia-income-employer-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-income-employer-verification-api-openapi.yml
- filename: sikoia-online-data-api-openapi.yml
  format: yaml
  label: Sikoia Online Data API
  slug: sikoia-online-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-online-data-api-openapi.yml
- filename: sikoia-peps-sanctions-api-openapi.yml
  format: yaml
  label: Sikoia PEPs & Sanctions API
  slug: sikoia-peps-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-peps-sanctions-api-openapi.yml
- filename: sikoia-user-management-api-openapi.yml
  format: yaml
  label: Sikoia User Management API
  slug: sikoia-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-user-management-api-openapi.yml
- filename: sikoia-validation-checklists-api-openapi.yml
  format: yaml
  label: Sikoia Validation Checklists API
  slug: sikoia-validation-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-validation-checklists-api-openapi.yml
- filename: sikoia-webhooks-api-openapi.yml
  format: yaml
  label: Sikoia Webhooks API
  slug: sikoia-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-webhooks-api-openapi.yml
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sikoia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sikoia secures its APIs with oauth2, http, and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sikoia
provider_slug: sikoia
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: authorizationHeader
  scheme: bearer
  sources:
  - openapi/sikoia-openapi.yml
  type: http
- deprecated: true
  end_of_support: '2025-11-30'
  in: header
  name: apiKeyHeader
  parameter: apikey
  sources:
  - openapi/sikoia-openapi.yml
  type: apiKey
slug: sikoia-authentication
source_filename: sikoia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sikoia.com/docs/authentication\ndocs: https://docs.sikoia.com/docs/authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  primary: oauth2 client_credentials (bearer JWT)\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: Migrated to OAuth 2.0. Legacy 'apikey' header auth deprecated; end of support 2025-11-30 (transitional\n    for pre-Jan-2024 customers).\noauth2:\n  flow: clientCredentials\n  token_url: https://oauth2.sikoia.com/token\n  token_url_staging: https://oauth2-staging.sikoia.com/token\n  scope: https://api.sikoia.com/.default\n  scope_staging: https://api-staging.sikoia.com/.default\n  token_format: JWT\n  token_expiry: 1 hour\n  client_secret_expiry: 2 years (rotatable; two secrets per application supported)\n  credential_management: https://portal.sikoia.com/Management/Applications\nschemes:\n- name: authorizationHeader\n  type: http\n  scheme: bearer\n \
  \ bearerFormat: JWT\n  sources:\n  - openapi/sikoia-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: apikey\n  deprecated: true\n  end_of_support: '2025-11-30'\n  sources:\n  - openapi/sikoia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/authentication/sikoia-authentication.yml
summary_line: oauth2/http/apiKey · 2 schemes
tags:
- Company
- Financial-Services
- Identity Verification
- KYC
- KYB
- Onboarding
- Open Banking
- Credit
- Affordability
- Fraud & AML
- Document Verification
- RegTech
---
