---
api_key_in: []
api_specs:
- filename: revenuecat-apps-api-openapi.yml
  format: yaml
  label: RevenueCat Apps API
  slug: revenuecat-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-apps-api-openapi.yml
- filename: revenuecat-customers-api-openapi.yml
  format: yaml
  label: RevenueCat Customers API
  slug: revenuecat-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-customers-api-openapi.yml
- filename: revenuecat-entitlements-v1-api-openapi.yml
  format: yaml
  label: RevenueCat Entitlements (v1) API
  slug: revenuecat-entitlements-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-entitlements-v1-api-openapi.yml
- filename: revenuecat-entitlements-v2-api-openapi.yml
  format: yaml
  label: RevenueCat Entitlements (v2) API
  slug: revenuecat-entitlements-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-entitlements-v2-api-openapi.yml
- filename: revenuecat-offerings-v1-api-openapi.yml
  format: yaml
  label: RevenueCat Offerings (v1) API
  slug: revenuecat-offerings-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-offerings-v1-api-openapi.yml
- filename: revenuecat-offerings-v2-api-openapi.yml
  format: yaml
  label: RevenueCat Offerings (v2) API
  slug: revenuecat-offerings-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-offerings-v2-api-openapi.yml
- filename: revenuecat-packages-api-openapi.yml
  format: yaml
  label: RevenueCat Packages API
  slug: revenuecat-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-packages-api-openapi.yml
- filename: revenuecat-products-api-openapi.yml
  format: yaml
  label: RevenueCat Products API
  slug: revenuecat-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-products-api-openapi.yml
- filename: revenuecat-projects-api-openapi.yml
  format: yaml
  label: RevenueCat Projects API
  slug: revenuecat-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-projects-api-openapi.yml
- filename: revenuecat-purchases-api-openapi.yml
  format: yaml
  label: RevenueCat Purchases API
  slug: revenuecat-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-purchases-api-openapi.yml
- filename: revenuecat-subscribers-api-openapi.yml
  format: yaml
  label: RevenueCat Subscribers API
  slug: revenuecat-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-subscribers-api-openapi.yml
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
- Subscription
- In-App Purchases
- Billing
- Mobile
- Entitlements
---
