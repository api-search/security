---
api_key_in:
- query
api_specs:
- filename: red-hat-3scale-accounts-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Accounts API
  slug: red-hat-3scale-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-accounts-api-openapi.yml
- filename: red-hat-3scale-applications-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Applications API
  slug: red-hat-3scale-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-applications-api-openapi.yml
- filename: red-hat-3scale-authorization-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Authorization API
  slug: red-hat-3scale-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-authorization-api-openapi.yml
- filename: red-hat-3scale-configuration-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Configuration API
  slug: red-hat-3scale-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-configuration-api-openapi.yml
- filename: red-hat-3scale-dns-api-openapi.yml
  format: yaml
  label: Red Hat 3scale DNS API
  slug: red-hat-3scale-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-dns-api-openapi.yml
- filename: red-hat-3scale-health-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Health API
  slug: red-hat-3scale-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-health-api-openapi.yml
- filename: red-hat-3scale-initialization-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Initialization API
  slug: red-hat-3scale-initialization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-initialization-api-openapi.yml
- filename: red-hat-3scale-invoices-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Invoices API
  slug: red-hat-3scale-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-invoices-api-openapi.yml
- filename: red-hat-3scale-oauth-api-openapi.yml
  format: yaml
  label: Red Hat 3scale OAuth API
  slug: red-hat-3scale-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-oauth-api-openapi.yml
- filename: red-hat-3scale-payment-transactions-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Payment Transactions API
  slug: red-hat-3scale-payment-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-payment-transactions-api-openapi.yml
- filename: red-hat-3scale-plans-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Plans API
  slug: red-hat-3scale-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-plans-api-openapi.yml
- filename: red-hat-3scale-reporting-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Reporting API
  slug: red-hat-3scale-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-reporting-api-openapi.yml
- filename: red-hat-3scale-services-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Services API
  slug: red-hat-3scale-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-services-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Red Hat 3Scale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Red Hat 3scale secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Red Hat 3scale
provider_slug: red-hat-3scale
scheme_count: 2
schemes:
- in: query
  name: provider_key
  parameter: access_token
  sources:
  - openapi/red-hat-3scale-account-management-openapi.yml
  - openapi/red-hat-3scale-analytics-openapi.yml
  - openapi/red-hat-3scale-billing-openapi.yml
  type: apiKey
- in: query
  name: providerKey
  parameter: provider_key
  sources:
  - openapi/red-hat-3scale-service-management-openapi.yml
  type: apiKey
slug: red-hat-3scale-authentication
source_filename: red-hat-3scale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/red-hat-3scale-account-management-openapi.yml, openapi/red-hat-3scale-analytics-openapi.yml,\n  openapi/red-hat-3scale-billing-openapi.yml, openapi/red-hat-3scale-service-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: provider_key\n  type: apiKey\n  in: query\n  parameter: access_token\n  sources:\n  - openapi/red-hat-3scale-account-management-openapi.yml\n  - openapi/red-hat-3scale-analytics-openapi.yml\n  - openapi/red-hat-3scale-billing-openapi.yml\n- name: providerKey\n  type: apiKey\n  in: query\n  parameter: provider_key\n  sources:\n  - openapi/red-hat-3scale-service-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/authentication/red-hat-3scale-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- API Gateway
- API Management
- Developer Portal
- Enterprise
- Red Hat
---
