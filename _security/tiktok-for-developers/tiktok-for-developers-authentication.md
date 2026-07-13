---
api_key_in: []
api_specs:
- filename: tiktok-display-openapi.yml
  format: yaml
  label: TikTok Display API
  slug: tiktok-display-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-display-openapi.yml
- filename: tiktok-content-posting-openapi.yml
  format: yaml
  label: TikTok Content Posting API
  slug: tiktok-content-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-content-posting-openapi.yml
- filename: tiktok-research-openapi.yml
  format: yaml
  label: TikTok Research API
  slug: tiktok-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-research-openapi.yml
- filename: tiktok-login-kit-openapi.yml
  format: yaml
  label: TikTok Login Kit
  slug: tiktok-login-kit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/openapi/tiktok-login-kit-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tiktok For Developers Authentication
name_suffix: Authentication
oauth_flows: []
overview: TikTok for Developers secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TikTok for Developers
provider_slug: tiktok-for-developers
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tiktok-content-posting-openapi.yml
  - openapi/tiktok-display-openapi.yml
  - openapi/tiktok-research-openapi.yml
  type: http
slug: tiktok-for-developers-authentication
source_filename: tiktok-for-developers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tiktok-content-posting-openapi.yml, openapi/tiktok-display-openapi.yml, openapi/tiktok-research-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token\n  sources:\n  - openapi/tiktok-content-posting-openapi.yml\n  - openapi/tiktok-display-openapi.yml\n  - openapi/tiktok-research-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiktok-for-developers/refs/heads/main/authentication/tiktok-for-developers-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- Analytics
- Authentication
- Content
- Social Media
- Video
---
