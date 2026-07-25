---
api_key_in:
- header
api_specs:
- filename: postiz-analytics-api-openapi.yml
  format: yaml
  label: Postiz Analytics API
  slug: postiz-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-analytics-api-openapi.yml
- filename: postiz-integrations-api-openapi.yml
  format: yaml
  label: Postiz Integrations API
  slug: postiz-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-integrations-api-openapi.yml
- filename: postiz-notifications-api-openapi.yml
  format: yaml
  label: Postiz Notifications API
  slug: postiz-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-notifications-api-openapi.yml
- filename: postiz-posts-api-openapi.yml
  format: yaml
  label: Postiz Posts API
  slug: postiz-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-posts-api-openapi.yml
- filename: postiz-uploads-api-openapi.yml
  format: yaml
  label: Postiz Uploads API
  slug: postiz-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-uploads-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Postiz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Postiz secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Postiz
provider_slug: postiz
scheme_count: 1
schemes:
- description: Your Postiz API key, sent as the raw value of the Authorization header.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/postiz-openapi.yml
  type: apiKey
slug: postiz-authentication
source_filename: postiz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/postiz-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Your Postiz API key, sent as the raw value of the Authorization header.\n  sources:\n  - openapi/postiz-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/authentication/postiz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social Media
- Scheduling
- Open Source
- Content
- Marketing
---
