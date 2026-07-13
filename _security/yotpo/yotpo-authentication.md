---
api_key_in:
- header
- query
api_specs:
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Reviews & Ratings API
  slug: yotpo-reviews-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Loyalty & Referrals API
  slug: yotpo-loyalty-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo SMS & Email API
  slug: yotpo-sms-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo UGC & Visual API
  slug: yotpo-ugc-visual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Subscriptions API
  slug: yotpo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Webhooks
  slug: yotpo-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Yotpo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yotpo secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yotpo
provider_slug: yotpo
scheme_count: 3
schemes:
- description: OAuth access token obtained from POST /oauth/token.
  in: query
  name: UToken
  parameter: utoken
  sources:
  - openapi/yotpo-openapi.yml
  type: apiKey
- description: Loyalty & Referrals account GUID.
  in: header
  name: LoyaltyGuid
  parameter: x-guid
  sources:
  - openapi/yotpo-openapi.yml
  type: apiKey
- description: Loyalty & Referrals API key.
  in: header
  name: LoyaltyApiKey
  parameter: x-api-key
  sources:
  - openapi/yotpo-openapi.yml
  type: apiKey
slug: yotpo-authentication
source_filename: yotpo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yotpo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: UToken\n  type: apiKey\n  in: query\n  parameter: utoken\n  description: OAuth access token obtained from POST /oauth/token.\n  sources:\n  - openapi/yotpo-openapi.yml\n- name: LoyaltyGuid\n  type: apiKey\n  in: header\n  parameter: x-guid\n  description: Loyalty & Referrals account GUID.\n  sources:\n  - openapi/yotpo-openapi.yml\n- name: LoyaltyApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Loyalty & Referrals API key.\n  sources:\n  - openapi/yotpo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/authentication/yotpo-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- eCommerce
- Reviews
- Loyalty
- Retention Marketing
- UGC
---
