---
api_key_in:
- header
api_specs:
- filename: tiktok-business-openapi.yml
  format: yaml
  label: TikTok API for Business
  slug: tiktok-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-business-openapi.yml
- filename: tiktok-shop-openapi.yml
  format: yaml
  label: TikTok Shop API
  slug: tiktok-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-shop-openapi.yml
- filename: tiktok-data-portability-openapi.yml
  format: yaml
  label: TikTok Data Portability API
  slug: tiktok-data-portability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-data-portability-openapi.yml
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
- Social Media
- Video
---
