---
api_key_in:
- header
api_specs:
- filename: tiktok-ad-groups-api-openapi.yml
  format: yaml
  label: TikTok Ad Groups API
  slug: tiktok-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-ad-groups-api-openapi.yml
- filename: tiktok-ads-api-openapi.yml
  format: yaml
  label: TikTok Ads API
  slug: tiktok-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-ads-api-openapi.yml
- filename: tiktok-audiences-api-openapi.yml
  format: yaml
  label: TikTok Audiences API
  slug: tiktok-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-audiences-api-openapi.yml
- filename: tiktok-campaigns-api-openapi.yml
  format: yaml
  label: TikTok Campaigns API
  slug: tiktok-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-campaigns-api-openapi.yml
- filename: tiktok-data-portability-api-openapi.yml
  format: yaml
  label: TikTok Data Portability API
  slug: tiktok-data-portability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-data-portability-api-openapi.yml
- filename: tiktok-finance-api-openapi.yml
  format: yaml
  label: TikTok Finance API
  slug: tiktok-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-finance-api-openapi.yml
- filename: tiktok-logistics-api-openapi.yml
  format: yaml
  label: TikTok Logistics API
  slug: tiktok-logistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-logistics-api-openapi.yml
- filename: tiktok-orders-api-openapi.yml
  format: yaml
  label: TikTok Orders API
  slug: tiktok-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-orders-api-openapi.yml
- filename: tiktok-products-api-openapi.yml
  format: yaml
  label: TikTok Products API
  slug: tiktok-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-products-api-openapi.yml
- filename: tiktok-reporting-api-openapi.yml
  format: yaml
  label: TikTok Reporting API
  slug: tiktok-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-reporting-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tiktok Authentication
name_suffix: Authentication
oauth_flows: []
overview: TikTok secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TikTok
provider_slug: tiktok
scheme_count: 3
schemes:
- description: TikTok Business API access token
  in: header
  name: AccessToken
  parameter: Access-Token
  sources:
  - openapi/tiktok-business-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tiktok-data-portability-openapi.yml
  type: http
- description: TikTok Shop API access token
  in: header
  name: AccessToken
  parameter: x-tts-access-token
  sources:
  - openapi/tiktok-shop-openapi.yml
  type: apiKey
slug: tiktok-authentication
source_filename: tiktok-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tiktok-business-openapi.yml, openapi/tiktok-data-portability-openapi.yml, openapi/tiktok-shop-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: Access-Token\n  description: TikTok Business API access token\n  sources:\n  - openapi/tiktok-business-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tiktok-data-portability-openapi.yml\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: x-tts-access-token\n  description: TikTok Shop API access token\n  sources:\n  - openapi/tiktok-shop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/authentication/tiktok-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Advertising
- Commerce
- Content
- E-Commerce
- Social-Media
- Video
---
