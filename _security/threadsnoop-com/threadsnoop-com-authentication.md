---
anonymous_access: false
api_key_in: []
api_specs:
- filename: threadsnoop-com-account-api-openapi.yml
  format: yaml
  label: threadsnoop-com Account API
  slug: threadsnoop-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/threadsnoop-com/openapi/threadsnoop-com-account-api-openapi.yml
- filename: threadsnoop-com-comments-api-openapi.yml
  format: yaml
  label: threadsnoop-com Comments API
  slug: threadsnoop-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/threadsnoop-com/openapi/threadsnoop-com-comments-api-openapi.yml
- filename: threadsnoop-com-posts-api-openapi.yml
  format: yaml
  label: threadsnoop-com Posts API
  slug: threadsnoop-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/threadsnoop-com/openapi/threadsnoop-com-posts-api-openapi.yml
- filename: threadsnoop-com-subreddits-api-openapi.yml
  format: yaml
  label: threadsnoop-com Subreddits API
  slug: threadsnoop-com-subreddits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/threadsnoop-com/openapi/threadsnoop-com-subreddits-api-openapi.yml
- filename: threadsnoop-com-users-api-openapi.yml
  format: yaml
  label: threadsnoop-com Users API
  slug: threadsnoop-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/threadsnoop-com/openapi/threadsnoop-com-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Threadsnoop Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: threadsnoop-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: threadsnoop-com
provider_slug: threadsnoop-com
scheme_count: 2
schemes:
- description: API key header
  in: header
  name: x-api-key
  type: apiKey
- description: 'Authorization: Bearer <your key> (equivalent to x-api-key)'
  scheme: bearer
  type: http
slug: threadsnoop-com-authentication
source_filename: threadsnoop-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://threadsnoop.com/docs/authentication\nschemes:\n  - type: apiKey\n    in: header\n    name: x-api-key\n    description: \"API key header\"\n  - type: http\n    scheme: bearer\n    description: \"Authorization: Bearer <your key> (equivalent to x-api-key)\"\n"
source_yaml_url: https://artifacts.apis.io/threadsnoop-com/authentication/threadsnoop-com-authentication.yml
summary_line: 2 schemes
tags:
- Reddit
- API
- AI
- MCP
- Read‑only
---
