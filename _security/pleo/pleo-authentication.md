---
api_key_in: []
api_specs:
- filename: pleo-bookkeeping-core-openapi.yml
  format: yaml
  label: Pleo Bookkeeping Core API
  slug: pleo-bookkeeping-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-bookkeeping-core-openapi.yml
- filename: pleo-gjoll-openapi.yml
  format: yaml
  label: Pleo Gjoll API
  slug: pleo-gjoll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-gjoll-openapi.yml
- filename: pleo-triton-openapi.yml
  format: yaml
  label: Pleo Triton API
  slug: pleo-triton-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-triton-openapi.yml
- filename: pleo-oberon-openapi.yml
  format: yaml
  label: Pleo Oberon API
  slug: pleo-oberon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-oberon-openapi.yml
- filename: pleo-export-openapi.yml
  format: yaml
  label: Pleo Export API
  slug: pleo-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-export-openapi.yml
- filename: pleo-tax-code-openapi.yml
  format: yaml
  label: Pleo Tax Code API
  slug: pleo-tax-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-tax-code-openapi.yml
- filename: pleo-tags-openapi.yml
  format: yaml
  label: Pleo Tags API
  slug: pleo-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-tags-openapi.yml
- filename: pleo-app-marketplace-openapi.yml
  format: yaml
  label: Pleo App Marketplace API
  slug: pleo-app-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-app-marketplace-openapi.yml
- filename: pleo-vendors-openapi.yml
  format: yaml
  label: Pleo Vendors API
  slug: pleo-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-vendors-openapi.yml
- filename: pleo-webhook-subscriptions-openapi.yml
  format: yaml
  label: Pleo Webhook Subscriptions API
  slug: pleo-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-webhook-subscriptions-openapi.yml
- filename: pleo-chart-of-accounts-openapi.yml
  format: yaml
  label: Pleo Chart of Accounts API
  slug: pleo-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-chart-of-accounts-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pleo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pleo secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pleo
provider_slug: pleo
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'JWT Bearer token authentication. Include the token in the Authorization header as: `Bearer <token>`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pleo-app-marketplace-openapi.yml
  - openapi/pleo-bookkeeping-core-openapi.yml
  - openapi/pleo-chart-of-accounts-openapi.yml
  - openapi/pleo-export-openapi.yml
  - openapi/pleo-gjoll-openapi.yml
  - openapi/pleo-oberon-openapi.yml
  - openapi/pleo-tags-openapi.yml
  - openapi/pleo-tax-code-openapi.yml
  - openapi/pleo-triton-openapi.yml
  - openapi/pleo-vendors-openapi.yml
  - openapi/pleo-webhook-subscriptions-openapi.yml
  type: http
- description: Basic HTTP authentication using API key. Use your API key as the username and leave the password empty. The credentials will be Base64 encoded automatically.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pleo-app-marketplace-openapi.yml
  - openapi/pleo-chart-of-accounts-openapi.yml
  - openapi/pleo-export-openapi.yml
  - openapi/pleo-gjoll-openapi.yml
  - openapi/pleo-oberon-openapi.yml
  - openapi/pleo-triton-openapi.yml
  - openapi/pleo-vendors-openapi.yml
  - openapi/pleo-webhook-subscriptions-openapi.yml
  type: http
slug: pleo-authentication
source_filename: pleo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pleo-app-marketplace-openapi.yml, openapi/pleo-bookkeeping-core-openapi.yml,\n  openapi/pleo-chart-of-accounts-openapi.yml, openapi/pleo-export-openapi.yml, openapi/pleo-gjoll-openapi.yml,\n  openapi/pleo-oberon-openapi.yml, openapi/pleo-tags-openapi.yml, openapi/pleo-tax-code-openapi.yml,\n  openapi/pleo-triton-openapi.yml, openapi/pleo-vendors-openapi.yml, openapi/pleo-webhook-subscriptions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT Bearer token authentication. Include the token in the Authorization header\n    as: `Bearer <token>`'\n  sources:\n  - openapi/pleo-app-marketplace-openapi.yml\n  - openapi/pleo-bookkeeping-core-openapi.yml\n  - openapi/pleo-chart-of-accounts-openapi.yml\n  - openapi/pleo-export-openapi.yml\n  - openapi/pleo-gjoll-openapi.yml\n  - openapi/pleo-oberon-openapi.yml\n  - openapi/pleo-tags-openapi.yml\n\
  \  - openapi/pleo-tax-code-openapi.yml\n  - openapi/pleo-triton-openapi.yml\n  - openapi/pleo-vendors-openapi.yml\n  - openapi/pleo-webhook-subscriptions-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic HTTP authentication using API key. Use your API key as the username and\n    leave the password empty. The credentials will be Base64 encoded automatically.\n  sources:\n  - openapi/pleo-app-marketplace-openapi.yml\n  - openapi/pleo-chart-of-accounts-openapi.yml\n  - openapi/pleo-export-openapi.yml\n  - openapi/pleo-gjoll-openapi.yml\n  - openapi/pleo-oberon-openapi.yml\n  - openapi/pleo-triton-openapi.yml\n  - openapi/pleo-vendors-openapi.yml\n  - openapi/pleo-webhook-subscriptions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/authentication/pleo-authentication.yml
summary_line: http · 2 schemes
tags:
- Expense Management
- Company Cards
- Spend Management
- Reimbursements
- Accounting
- FinTech
- Finance
---
