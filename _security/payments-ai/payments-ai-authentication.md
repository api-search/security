---
anonymous_access: false
api_key_in: []
api_specs:
- filename: payments-ai-api-keys-api-openapi.yml
  format: yaml
  label: payments-ai API Keys API
  slug: payments-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-api-keys-api-openapi.yml
- filename: payments-ai-buyer-checkout-api-openapi.yml
  format: yaml
  label: payments-ai Buyer checkout API
  slug: payments-ai-buyer-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-buyer-checkout-api-openapi.yml
- filename: payments-ai-checkout-api-openapi.yml
  format: yaml
  label: payments-ai Checkout API
  slug: payments-ai-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-checkout-api-openapi.yml
- filename: payments-ai-customers-api-openapi.yml
  format: yaml
  label: payments-ai Customers API
  slug: payments-ai-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-customers-api-openapi.yml
- filename: payments-ai-invoices-api-openapi.yml
  format: yaml
  label: payments-ai Invoices API
  slug: payments-ai-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-invoices-api-openapi.yml
- filename: payments-ai-json-api-openapi.yml
  format: yaml
  label: payments-ai JSON API
  slug: payments-ai-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-json-api-openapi.yml
- filename: payments-ai-markdown-api-openapi.yml
  format: yaml
  label: payments-ai Markdown API
  slug: payments-ai-markdown-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-markdown-api-openapi.yml
- filename: payments-ai-merchant-api-openapi.yml
  format: yaml
  label: payments-ai Merchant API
  slug: payments-ai-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-merchant-api-openapi.yml
- filename: payments-ai-orders-api-openapi.yml
  format: yaml
  label: payments-ai Orders API
  slug: payments-ai-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-orders-api-openapi.yml
- filename: payments-ai-pages-api-openapi.yml
  format: yaml
  label: payments-ai Pages API
  slug: payments-ai-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-pages-api-openapi.yml
- filename: payments-ai-products-api-openapi.yml
  format: yaml
  label: payments-ai Products API
  slug: payments-ai-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-products-api-openapi.yml
- filename: payments-ai-public-api-api-openapi.yml
  format: yaml
  label: payments-ai Public API
  slug: payments-ai-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-public-api-api-openapi.yml
- filename: payments-ai-subscriptions-api-openapi.yml
  format: yaml
  label: payments-ai Subscriptions API
  slug: payments-ai-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-subscriptions-api-openapi.yml
- filename: payments-ai-transactions-api-openapi.yml
  format: yaml
  label: payments-ai Transactions API
  slug: payments-ai-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Payments Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: payments-ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: payments-ai
provider_slug: payments-ai
scheme_count: 1
schemes:
- description: 'Signed-in user OAuth credential (`pai_mcp_*`) issued through the dashboard consent screen for this API: the authorization and token requests name the RFC 8707 resource `<API_URL>/v1/public-api` (ADR-0020). Credentials issued for the MCP server, or for no resource, are rejected with 401 `auth.invalid_token` and `WWW-Authenticate: Bearer resource_metadata="<API_URL>/.well-known/oauth-protected-resou'
  name: UserOAuthCredentialAuth
  scheme: Bearer
  sources:
  - openapi/payments-ai-mor-openapi.json
  type: http
slug: payments-ai-authentication
source_filename: payments-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/payments-ai-mor-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: UserOAuthCredentialAuth\n  type: http\n  scheme: Bearer\n  description: 'Signed-in user OAuth credential (`pai_mcp_*`) issued through the dashboard consent\n    screen for this API: the authorization and token requests name the RFC 8707 resource `<API_URL>/v1/public-api`\n    (ADR-0020). Credentials issued for the MCP server, or for no resource, are rejected with\n    401 `auth.invalid_token` and `WWW-Authenticate: Bearer resource_metadata=\"<API_URL>/.well-known/oauth-protected-resou'\n  sources:\n  - openapi/payments-ai-mor-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/payments-ai/authentication/payments-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- AI
- FinTech
- Merchant of Record
- Payment Orchestration
---
