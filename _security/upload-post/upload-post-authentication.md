---
api_key_in:
- header
api_specs:
- filename: upload-post-analytics-api-openapi.yml
  format: yaml
  label: Upload-Post Analytics API
  slug: upload-post-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-analytics-api-openapi.yml
- filename: upload-post-upload-api-openapi.yml
  format: yaml
  label: Upload-Post Upload API
  slug: upload-post-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-upload-api-openapi.yml
- filename: upload-post-upload-management-api-openapi.yml
  format: yaml
  label: Upload-Post Upload Management API
  slug: upload-post-upload-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-upload-management-api-openapi.yml
- filename: upload-post-users-api-openapi.yml
  format: yaml
  label: Upload-Post Users API
  slug: upload-post-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Upload Post Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upload-Post secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Upload-Post
provider_slug: upload-post
scheme_count: 1
schemes:
- description: 'API key authentication. Provide the header in the form `Authorization: Apikey YOUR_API_KEY`.'
  in: header
  name: ApikeyAuth
  parameter: Authorization
  sources:
  - openapi/upload-post-openapi.yml
  type: apiKey
slug: upload-post-authentication
source_filename: upload-post-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/upload-post-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApikeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication. Provide the header in the form `Authorization: Apikey\n    YOUR_API_KEY`.'\n  sources:\n  - openapi/upload-post-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/authentication/upload-post-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social-Media
- Publishing
- Video
- Content
- Cross Posting
---
