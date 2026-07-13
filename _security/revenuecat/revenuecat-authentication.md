---
api_key_in: []
api_specs:
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Subscribers API
  slug: revenuecat-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Purchases & Receipts API
  slug: revenuecat-purchases-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Entitlements API (v1)
  slug: revenuecat-entitlements-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Offerings API (v1)
  slug: revenuecat-offerings-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Customer Attributes API
  slug: revenuecat-customer-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Projects API (v2)
  slug: revenuecat-projects-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Apps API (v2)
  slug: revenuecat-apps-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Customers API (v2)
  slug: revenuecat-customers-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Products API (v2)
  slug: revenuecat-products-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Entitlements API (v2)
  slug: revenuecat-entitlements-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Offerings API (v2)
  slug: revenuecat-offerings-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Packages API (v2)
  slug: revenuecat-packages-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Revenuecat Authentication
name_suffix: Authentication
oauth_flows: []
overview: RevenueCat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RevenueCat
provider_slug: revenuecat
scheme_count: 1
schemes:
- description: RevenueCat API key passed as an HTTP Bearer token. v1 accepts public (client) or secret (server) keys; v2 uses dedicated v2 API keys.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/revenuecat-openapi.yml
  type: http
slug: revenuecat-authentication
source_filename: revenuecat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revenuecat-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: RevenueCat API key passed as an HTTP Bearer token. v1 accepts public (client)\n    or secret (server) keys; v2 uses dedicated v2 API keys.\n  sources:\n  - openapi/revenuecat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/authentication/revenuecat-authentication.yml
summary_line: http · 1 scheme
tags:
- Subscriptions
- In-App Purchases
- Billing
- Mobile
- Entitlements
---
