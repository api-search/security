---
api_key_in:
- header
api_specs:
- filename: dopost-co-media-api-openapi.yml
  format: yaml
  label: dopost Media API
  slug: dopost-co-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopost-co/refs/heads/main/openapi/dopost-co-media-api-openapi.yml
- filename: dopost-co-posts-api-openapi.yml
  format: yaml
  label: dopost Posts API
  slug: dopost-co-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopost-co/refs/heads/main/openapi/dopost-co-posts-api-openapi.yml
- filename: dopost-co-social-accounts-api-openapi.yml
  format: yaml
  label: dopost Social Accounts API
  slug: dopost-co-social-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopost-co/refs/heads/main/openapi/dopost-co-social-accounts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dopost Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: dopost secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dopost
provider_slug: dopost-co
scheme_count: 1
schemes:
- description: Workspace API key issued from the dopost web app.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/dopost-openapi.yml
  type: apiKey
slug: dopost-co-authentication
source_filename: dopost-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dopost-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Workspace API key issued from the dopost web app.\n  sources:\n  - openapi/dopost-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dopost-co/refs/heads/main/authentication/dopost-co-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social Media
- Scheduling
- Publishing
- Instagram
- Facebook
- TikTok
- Pinterest
- X Twitter
- YouTube
- Content Management
- REST
---
