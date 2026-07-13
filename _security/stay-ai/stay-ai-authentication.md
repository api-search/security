---
api_key_in:
- header
api_specs:
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Subscriptions API
  slug: stay-ai-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Subscription Orders API
  slug: stay-ai-subscription-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Selling Plans API
  slug: stay-ai-selling-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Catalog API
  slug: stay-ai-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Customer Portal API
  slug: stay-ai-customer-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Webhooks API
  slug: stay-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Account and Data API
  slug: stay-ai-account-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stay Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stay AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stay AI
provider_slug: stay-ai
scheme_count: 1
schemes:
- in: header
  name: accessToken
  parameter: X-RETEXTION-ACCESS-TOKEN
  sources:
  - openapi/stay-ai-openapi.yml
  type: apiKey
slug: stay-ai-authentication
source_filename: stay-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stay-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: X-RETEXTION-ACCESS-TOKEN\n  sources:\n  - openapi/stay-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/authentication/stay-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Subscriptions
- Retention
- Churn
- Shopify
- Ecommerce
- DTC
---
