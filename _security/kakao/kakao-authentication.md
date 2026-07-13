---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kakao Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kakao secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kakao
provider_slug: kakao
scheme_count: 2
schemes:
- bearerFormat: Kakao access token
  description: Kakao access token issued by /oauth/token, sent as "Bearer {access_token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kakao-openapi.yml
  type: http
- description: Kakao app Admin Key sent as "KakaoAK {admin_key}" for server-to-server calls.
  in: header
  name: adminKey
  parameter: Authorization
  sources:
  - openapi/kakao-openapi.yml
  type: apiKey
slug: kakao-authentication
source_filename: kakao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kakao-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Kakao access token\n  description: Kakao access token issued by /oauth/token, sent as \"Bearer {access_token}\".\n  sources:\n  - openapi/kakao-openapi.yml\n- name: adminKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Kakao app Admin Key sent as \"KakaoAK {admin_key}\" for server-to-server calls.\n  sources:\n  - openapi/kakao-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kakao/refs/heads/main/authentication/kakao-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Messaging
- Maps
- Navigation
- Payments
- Search
- Korea
- Identity
- OAuth2
- KakaoTalk
- LLM
---
