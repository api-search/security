---
api_key_in:
- header
api_specs:
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Customers API
  slug: skimmer-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Bodies of Water API
  slug: skimmer-bodies-of-water-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Service Locations API
  slug: skimmer-service-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Work Orders API
  slug: skimmer-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Routes API
  slug: skimmer-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Invoices and Billing API
  slug: skimmer-invoices-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Quotes API
  slug: skimmer-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Products API
  slug: skimmer-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Users API
  slug: skimmer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Skimmer Pool Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skimmer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Skimmer
provider_slug: skimmer-pool
scheme_count: 1
schemes:
- description: Per-account Skimmer Public API key, issued via sales-led onboarding.
  in: header
  name: skimmerApiKey
  parameter: skimmer-api-key
  sources:
  - openapi/skimmer-pool-openapi.yml
  type: apiKey
slug: skimmer-pool-authentication
source_filename: skimmer-pool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/skimmer-pool-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: skimmerApiKey\n  type: apiKey\n  in: header\n  parameter: skimmer-api-key\n  description: Per-account Skimmer Public API key, issued via sales-led onboarding.\n  sources:\n  - openapi/skimmer-pool-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/authentication/skimmer-pool-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Pool Service
- Field Service Management
- Pool Maintenance
- Scheduling
- Routes
- Work Orders
- Invoicing
- Vertical SaaS
---
