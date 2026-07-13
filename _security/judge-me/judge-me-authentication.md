---
api_key_in:
- query
api_specs:
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Reviews API
  slug: judge-me-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Reviewers API
  slug: judge-me-reviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Products API
  slug: judge-me-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Widgets API
  slug: judge-me-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me OAuth API
  slug: judge-me-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Webhooks API
  slug: judge-me-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Judge Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Judge.me secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Judge.me
provider_slug: judge-me
scheme_count: 2
schemes:
- description: Public or private Judge.me API token passed as a query parameter.
  in: query
  name: apiToken
  parameter: api_token
  sources:
  - openapi/judge-me-openapi.yml
  type: apiKey
- description: The store's myshopify.com domain passed as a query parameter.
  in: query
  name: shopDomain
  parameter: shop_domain
  sources:
  - openapi/judge-me-openapi.yml
  type: apiKey
slug: judge-me-authentication
source_filename: judge-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/judge-me-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: Public or private Judge.me API token passed as a query parameter.\n  sources:\n  - openapi/judge-me-openapi.yml\n- name: shopDomain\n  type: apiKey\n  in: query\n  parameter: shop_domain\n  description: The store's myshopify.com domain passed as a query parameter.\n  sources:\n  - openapi/judge-me-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/authentication/judge-me-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Reviews
- E-commerce
- Shopify
- Ratings
- Social Proof
---
