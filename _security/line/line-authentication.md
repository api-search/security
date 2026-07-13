---
api_key_in: []
api_specs:
- filename: messaging-api.yml
  format: yaml
  label: LINE Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/messaging-api.yml
- filename: liff.yml
  format: yaml
  label: LINE Front-end Framework (LIFF) Server API
  slug: liff
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/liff.yml
- filename: channel-access-token.yml
  format: yaml
  label: LINE Channel Access Token API
  slug: channel-access-token
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/channel-access-token.yml
- filename: insight.yml
  format: yaml
  label: LINE Insight API
  slug: insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/insight.yml
- filename: manage-audience.yml
  format: yaml
  label: LINE Manage Audience API
  slug: manage-audience
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/manage-audience.yml
- filename: shop.yml
  format: yaml
  label: LINE Shop (Mission Stickers) API
  slug: shop
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/shop.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Line Authentication
name_suffix: Authentication
oauth_flows: []
overview: LINE secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LINE
provider_slug: line
scheme_count: 1
schemes:
- bearerFormat: ChannelAccessToken
  description: LINE channel access token passed as a Bearer token in the Authorization header.
  name: ChannelAccessToken
  scheme: bearer
  sources:
  - openapi/line-openapi.yml
  type: http
slug: line-authentication
source_filename: line-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/line-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ChannelAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: ChannelAccessToken\n  description: LINE channel access token passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/line-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/authentication/line-authentication.yml
summary_line: http · 1 scheme
tags:
- Messaging
- Chatbots
- Social Login
- Mini Apps
- Marketing
- Japan
---
