---
api_key_in: []
api_specs:
- filename: line-channel-api-openapi.yml
  format: yaml
  label: LINE Channel API
  slug: line-channel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-channel-api-openapi.yml
- filename: line-info-api-openapi.yml
  format: yaml
  label: LINE Info API
  slug: line-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-info-api-openapi.yml
- filename: line-message-api-openapi.yml
  format: yaml
  label: LINE Message API
  slug: line-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-message-api-openapi.yml
- filename: line-profile-api-openapi.yml
  format: yaml
  label: LINE Profile API
  slug: line-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-profile-api-openapi.yml
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
