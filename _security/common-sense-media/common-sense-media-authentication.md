---
api_key_in:
- header
api_specs:
- filename: common-sense-media-reviews-api-openapi.yml
  format: yaml
  label: Common Sense Media Reviews API
  slug: common-sense-media-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/common-sense-media/refs/heads/main/openapi/common-sense-media-reviews-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Common Sense Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Common Sense Media secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Common Sense Media
provider_slug: common-sense-media
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - openapi/common-sense-media-reviews-api-openapi.yml
  type: apiKey
slug: common-sense-media-authentication
source_filename: common-sense-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/common-sense-media-reviews-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/common-sense-media-reviews-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/common-sense-media/refs/heads/main/authentication/common-sense-media-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Apps
- Books
- Media
- Movies
- Non-Profit
- Podcasts
- Ratings
- Reviews
- Television
- Video Games
- YouTube
---
