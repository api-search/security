---
api_key_in: []
api_specs:
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Customers API
  slug: smile-io-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Points Transactions API
  slug: smile-io-points-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Points Products API
  slug: smile-io-points-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Reward Fulfillments API
  slug: smile-io-rewards-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Earning Rules API
  slug: smile-io-earning-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io VIP Tiers API
  slug: smile-io-vip-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Activities API
  slug: smile-io-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smile Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smile.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smile.io
provider_slug: smile-io
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smile-io-openapi.yml
  type: http
slug: smile-io-authentication
source_filename: smile-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smile-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/smile-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/authentication/smile-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Loyalty
- Rewards
- Referrals
- E-commerce
- Points
- Customer Retention
- Shopify
---
