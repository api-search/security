---
api_key_in:
- header
api_specs:
- filename: kintsugi-address-validation-api-openapi.yml
  format: yaml
  label: Kintsugi Address Validation API
  slug: kintsugi-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-address-validation-api-openapi.yml
- filename: kintsugi-customers-api-openapi.yml
  format: yaml
  label: Kintsugi Customers API
  slug: kintsugi-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-customers-api-openapi.yml
- filename: kintsugi-exemptions-api-openapi.yml
  format: yaml
  label: Kintsugi Exemptions API
  slug: kintsugi-exemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-exemptions-api-openapi.yml
- filename: kintsugi-filings-api-openapi.yml
  format: yaml
  label: Kintsugi Filings API
  slug: kintsugi-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-filings-api-openapi.yml
- filename: kintsugi-nexus-api-openapi.yml
  format: yaml
  label: Kintsugi Nexus API
  slug: kintsugi-nexus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-nexus-api-openapi.yml
- filename: kintsugi-products-api-openapi.yml
  format: yaml
  label: Kintsugi Products API
  slug: kintsugi-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-products-api-openapi.yml
- filename: kintsugi-registrations-api-openapi.yml
  format: yaml
  label: Kintsugi Registrations API
  slug: kintsugi-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-registrations-api-openapi.yml
- filename: kintsugi-tax-estimation-api-openapi.yml
  format: yaml
  label: Kintsugi Tax Estimation API
  slug: kintsugi-tax-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-tax-estimation-api-openapi.yml
- filename: kintsugi-transactions-api-openapi.yml
  format: yaml
  label: Kintsugi Transactions API
  slug: kintsugi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kintsugi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kintsugi secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kintsugi
provider_slug: kintsugi
scheme_count: 2
schemes:
- description: API key generated in the Kintsugi dashboard.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/kintsugi-openapi.yml
  type: apiKey
- description: Identifier of the organization the request acts on behalf of.
  in: header
  name: OrganizationId
  parameter: x-organization-id
  sources:
  - openapi/kintsugi-openapi.yml
  type: apiKey
slug: kintsugi-authentication
source_filename: kintsugi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kintsugi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key generated in the Kintsugi dashboard.\n  sources:\n  - openapi/kintsugi-openapi.yml\n- name: OrganizationId\n  type: apiKey\n  in: header\n  parameter: x-organization-id\n  description: Identifier of the organization the request acts on behalf of.\n  sources:\n  - openapi/kintsugi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/authentication/kintsugi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Sales Tax
- Tax Compliance
- Tax Automation
- VAT
- GST
- Nexus
- Artificial Intelligence
---
