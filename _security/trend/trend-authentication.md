---
api_key_in:
- header
api_specs:
- filename: trend-ai-api-openapi.yml
  format: yaml
  label: Trend AI API
  slug: trend-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-ai-api-openapi.yml
- filename: trend-auth-api-openapi.yml
  format: yaml
  label: Trend Auth API
  slug: trend-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-auth-api-openapi.yml
- filename: trend-basic-authentication-ai-api-openapi.yml
  format: yaml
  label: Trend Basic Authentication (AI) API
  slug: trend-basic-authentication-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-basic-authentication-ai-api-openapi.yml
- filename: trend-brand-admin-api-openapi.yml
  format: yaml
  label: Trend Brand Admin API
  slug: trend-brand-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-brand-admin-api-openapi.yml
- filename: trend-brand-api-openapi.yml
  format: yaml
  label: Trend Brand API
  slug: trend-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-brand-api-openapi.yml
- filename: trend-brand-authentication-api-openapi.yml
  format: yaml
  label: Trend Brand Authentication API
  slug: trend-brand-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-brand-authentication-api-openapi.yml
- filename: trend-campaign-api-openapi.yml
  format: yaml
  label: Trend Campaign API
  slug: trend-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-campaign-api-openapi.yml
- filename: trend-content-api-openapi.yml
  format: yaml
  label: Trend Content API
  slug: trend-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-content-api-openapi.yml
- filename: trend-creator-api-openapi.yml
  format: yaml
  label: Trend Creator API
  slug: trend-creator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-creator-api-openapi.yml
- filename: trend-creator-authentication-api-openapi.yml
  format: yaml
  label: Trend Creator Authentication API
  slug: trend-creator-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-creator-authentication-api-openapi.yml
- filename: trend-creator-portfolio-api-openapi.yml
  format: yaml
  label: Trend Creator Portfolio API
  slug: trend-creator-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-creator-portfolio-api-openapi.yml
- filename: trend-creator-profiles-api-openapi.yml
  format: yaml
  label: Trend Creator Profiles API
  slug: trend-creator-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-creator-profiles-api-openapi.yml
- filename: trend-health-check-api-openapi.yml
  format: yaml
  label: Trend Health Check API
  slug: trend-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-health-check-api-openapi.yml
- filename: trend-message-api-openapi.yml
  format: yaml
  label: Trend Message API
  slug: trend-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-message-api-openapi.yml
- filename: trend-metrics-api-openapi.yml
  format: yaml
  label: Trend Metrics API
  slug: trend-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-metrics-api-openapi.yml
- filename: trend-partnership-api-openapi.yml
  format: yaml
  label: Trend Partnership API
  slug: trend-partnership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-partnership-api-openapi.yml
- filename: trend-payment-api-openapi.yml
  format: yaml
  label: Trend Payment API
  slug: trend-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-payment-api-openapi.yml
- filename: trend-review-api-openapi.yml
  format: yaml
  label: Trend Review API
  slug: trend-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-review-api-openapi.yml
- filename: trend-shipment-api-openapi.yml
  format: yaml
  label: Trend Shipment API
  slug: trend-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-shipment-api-openapi.yml
- filename: trend-upload-api-openapi.yml
  format: yaml
  label: Trend Upload API
  slug: trend-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-upload-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trend secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trend
provider_slug: trend
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: access-token
  scheme: bearer
  sources:
  - openapi/trend-api-openapi.yml
  type: http
- in: header
  name: admin-api-key
  parameter: trend-api-key
  sources:
  - openapi/trend-api-openapi.yml
  type: apiKey
slug: trend-authentication
source_filename: trend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/trend-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: access-token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/trend-api-openapi.yml\n- name: admin-api-key\n  type: apiKey\n  in: header\n  parameter: trend-api-key\n  sources:\n  - openapi/trend-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/authentication/trend-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- User-Generated Content
- Creator Economy
- Content Marketing
- Video Production
- Photography
- Marketing
- E-Commerce
- Creator Marketplace
- Influencer Marketing
- AI Image Generation
- Payments
---
