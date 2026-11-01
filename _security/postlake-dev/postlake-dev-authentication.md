---
anonymous_access: false
api_key_in: []
api_specs:
- filename: postlake-dev-account-api-openapi.yml
  format: yaml
  label: postlake-dev Account API
  slug: postlake-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-account-api-openapi.yml
- filename: postlake-dev-analytics-api-openapi.yml
  format: yaml
  label: postlake-dev Analytics API
  slug: postlake-dev-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-analytics-api-openapi.yml
- filename: postlake-dev-channels-api-openapi.yml
  format: yaml
  label: postlake-dev Channels API
  slug: postlake-dev-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-channels-api-openapi.yml
- filename: postlake-dev-connect-api-openapi.yml
  format: yaml
  label: postlake-dev Connect API
  slug: postlake-dev-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-connect-api-openapi.yml
- filename: postlake-dev-credentials-api-openapi.yml
  format: yaml
  label: postlake-dev Credentials API
  slug: postlake-dev-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-credentials-api-openapi.yml
- filename: postlake-dev-discovery-api-openapi.yml
  format: yaml
  label: postlake-dev Discovery API
  slug: postlake-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-discovery-api-openapi.yml
- filename: postlake-dev-engaging-api-openapi.yml
  format: yaml
  label: postlake-dev Engaging API
  slug: postlake-dev-engaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-engaging-api-openapi.yml
- filename: postlake-dev-live-video-api-openapi.yml
  format: yaml
  label: postlake-dev Live Video API
  slug: postlake-dev-live-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-live-video-api-openapi.yml
- filename: postlake-dev-mcp-api-openapi.yml
  format: yaml
  label: postlake-dev MCP API
  slug: postlake-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-mcp-api-openapi.yml
- filename: postlake-dev-media-api-openapi.yml
  format: yaml
  label: postlake-dev Media API
  slug: postlake-dev-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-media-api-openapi.yml
- filename: postlake-dev-messages-api-openapi.yml
  format: yaml
  label: postlake-dev Messages API
  slug: postlake-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-messages-api-openapi.yml
- filename: postlake-dev-openapi-json-api-openapi.yml
  format: yaml
  label: postlake-dev Openapi.json API
  slug: postlake-dev-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-openapi-json-api-openapi.yml
- filename: postlake-dev-platform-api-openapi.yml
  format: yaml
  label: postlake-dev Platform API
  slug: postlake-dev-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-platform-api-openapi.yml
- filename: postlake-dev-platforms-api-openapi.yml
  format: yaml
  label: postlake-dev Platforms API
  slug: postlake-dev-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-platforms-api-openapi.yml
- filename: postlake-dev-posts-api-openapi.yml
  format: yaml
  label: postlake-dev Posts API
  slug: postlake-dev-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-posts-api-openapi.yml
- filename: postlake-dev-profiles-api-openapi.yml
  format: yaml
  label: postlake-dev Profiles API
  slug: postlake-dev-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-profiles-api-openapi.yml
- filename: postlake-dev-reading-api-openapi.yml
  format: yaml
  label: postlake-dev Reading API
  slug: postlake-dev-reading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-reading-api-openapi.yml
- filename: postlake-dev-social-accounts-api-openapi.yml
  format: yaml
  label: postlake-dev Social Accounts API
  slug: postlake-dev-social-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-social-accounts-api-openapi.yml
- filename: postlake-dev-webhooks-api-openapi.yml
  format: yaml
  label: postlake-dev Webhooks API
  slug: postlake-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postlake-dev/openapi/postlake-dev-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Postlake Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: postlake-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: postlake-dev
provider_slug: postlake-dev
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token authentication using API key prefixed with 'sk_live_'.
  in: header
  name: Authorization
  type: apiKey
slug: postlake-dev-authentication
source_filename: postlake-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.postlake.dev/authentication.md\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token authentication using API key prefixed with 'sk_live_'.\"\n    bearerFormat: JWT\n"
source_yaml_url: https://artifacts.apis.io/postlake-dev/authentication/postlake-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Media
- API
- AI Agents
- MCP
- SaaS
- Automation
- Publishing
---
