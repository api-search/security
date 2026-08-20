---
api_key_in:
- header
api_specs:
- filename: dealhub-quote-api-openapi.yml
  format: yaml
  label: DealHub Quote API
  slug: dealhub-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-quote-api-openapi.yml
- filename: dealhub-headless-api-openapi.yml
  format: yaml
  label: DealHub Headless Quote API
  slug: dealhub-headless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-headless-api-openapi.yml
- filename: dealhub-crm-api-openapi.yml
  format: yaml
  label: DealHub CRM API
  slug: dealhub-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-crm-api-openapi.yml
- filename: dealhub-crm-import-api-openapi.yml
  format: yaml
  label: DealHub CRM Import API
  slug: dealhub-crm-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-crm-import-api-openapi.yml
- filename: dealhub-user-api-openapi.yml
  format: yaml
  label: DealHub User API
  slug: dealhub-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-user-api-openapi.yml
- filename: dealhub-partner-api-openapi.yml
  format: yaml
  label: DealHub Partner API
  slug: dealhub-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-partner-api-openapi.yml
- filename: dealhub-pricing-api-openapi.yml
  format: yaml
  label: DealHub Pricing API
  slug: dealhub-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-pricing-api-openapi.yml
- filename: dealhub-version-api-openapi.yml
  format: yaml
  label: DealHub Version API
  slug: dealhub-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-version-api-openapi.yml
- filename: dealhub-subskribe-api-openapi.yml
  format: yaml
  label: DealHub Subskribe API
  slug: dealhub-subskribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-subskribe-api-openapi.yml
- filename: dealhub-external-query-openapi.yml
  format: yaml
  label: DealHub External Query (inbound callback contract)
  slug: dealhub-external-query
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-external-query-openapi.yml
- filename: dealhub-callout-api-openapi.yml
  format: yaml
  label: DealHub Callout API (inbound callback contract)
  slug: dealhub-callout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-callout-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dealhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: DealHub secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DealHub
provider_slug: dealhub
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Bearer token authentication. The token is provided by the DealHub admin during Callout configuration.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dealhub-callout-api-openapi.yml
  - openapi/dealhub-crm-api-openapi.yml
  - openapi/dealhub-crm-import-api-openapi.yml
  - openapi/dealhub-external-query-openapi.yml
  - openapi/dealhub-headless-api-openapi.yml
  - openapi/dealhub-partner-api-openapi.yml
  - openapi/dealhub-pricing-api-openapi.yml
  - openapi/dealhub-quote-api-openapi.yml
  - openapi/dealhub-user-api-openapi.yml
  - openapi/dealhub-version-api-openapi.yml
  type: http
- description: Basic authentication with username and password. Credentials are provided by the DealHub admin during Callout configuration.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/dealhub-callout-api-openapi.yml
  - openapi/dealhub-external-query-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/dealhub-subskribe-api-openapi.yml
  type: apiKey
slug: dealhub-authentication
source_filename: dealhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/dealhub-callout-api-openapi.yml, openapi/dealhub-crm-api-openapi.yml, openapi/dealhub-crm-import-api-openapi.yml,\n  openapi/dealhub-external-query-openapi.yml, openapi/dealhub-headless-api-openapi.yml, openapi/dealhub-partner-api-openapi.yml,\n  openapi/dealhub-pricing-api-openapi.yml, openapi/dealhub-quote-api-openapi.yml, openapi/dealhub-subskribe-api-openapi.yml,\n  openapi/dealhub-user-api-openapi.yml, openapi/dealhub-version-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication. The token is provided by the DealHub admin during\n    Callout configuration.\n  sources:\n  - openapi/dealhub-callout-api-openapi.yml\n  - openapi/dealhub-crm-api-openapi.yml\n  - openapi/dealhub-crm-import-api-openapi.yml\n  - openapi/dealhub-external-query-openapi.yml\n  - openapi/dealhub-headless-api-openapi.yml\n\
  \  - openapi/dealhub-partner-api-openapi.yml\n  - openapi/dealhub-pricing-api-openapi.yml\n  - openapi/dealhub-quote-api-openapi.yml\n  - openapi/dealhub-user-api-openapi.yml\n  - openapi/dealhub-version-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with username and password. Credentials are provided by\n    the DealHub admin during Callout configuration.\n  sources:\n  - openapi/dealhub-callout-api-openapi.yml\n  - openapi/dealhub-external-query-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/dealhub-subskribe-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/authentication/dealhub-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- CPQ
- Quote-to-Cash
- Contract Lifecycle Management
- Subscription Management
- Billing
- Revenue Operations
- Sales
- Pricing
- Usage-Based Billing
- Revenue Recognition
- Sales Enablement
---
