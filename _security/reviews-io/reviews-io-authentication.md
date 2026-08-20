---
api_key_in:
- header
api_specs:
- filename: reviews-io-company-reviews-api-openapi.yml
  format: yaml
  label: REVIEWS.io Company Reviews API
  slug: reviews-io-company-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-company-reviews-api-openapi.yml
- filename: reviews-io-invitations-api-openapi.yml
  format: yaml
  label: REVIEWS.io Invitations API
  slug: reviews-io-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-invitations-api-openapi.yml
- filename: reviews-io-product-reviews-api-openapi.yml
  format: yaml
  label: REVIEWS.io Product Reviews API
  slug: reviews-io-product-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-product-reviews-api-openapi.yml
- filename: reviews-io-questions-api-openapi.yml
  format: yaml
  label: REVIEWS.io Questions API
  slug: reviews-io-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-questions-api-openapi.yml
- filename: reviews-io-ratings-api-openapi.yml
  format: yaml
  label: REVIEWS.io Ratings API
  slug: reviews-io-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-ratings-api-openapi.yml
- filename: reviews-io-webhooks-api-openapi.yml
  format: yaml
  label: REVIEWS.io Webhooks API
  slug: reviews-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reviews Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: REVIEWS.io secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: REVIEWS.io
provider_slug: reviews-io
scheme_count: 2
schemes:
- description: Your REVIEWS.io public store key.
  in: header
  name: storeKey
  parameter: store
  sources:
  - openapi/reviews-io-openapi.yml
  type: apiKey
- description: Your REVIEWS.io private API key.
  in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/reviews-io-openapi.yml
  type: apiKey
slug: reviews-io-authentication
source_filename: reviews-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reviews-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: storeKey\n  type: apiKey\n  in: header\n  parameter: store\n  description: Your REVIEWS.io public store key.\n  sources:\n  - openapi/reviews-io-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Your REVIEWS.io private API key.\n  sources:\n  - openapi/reviews-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/authentication/reviews-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Reviews
- UGC
- Ratings
- Reputation
- E-Commerce
---
