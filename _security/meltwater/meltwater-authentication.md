---
api_key_in:
- header
api_specs:
- filename: meltwater-account-management-api-openapi.yml
  format: yaml
  label: Meltwater Account Management API
  slug: meltwater-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-account-management-api-openapi.yml
- filename: meltwater-bring-your-own-content-byoc-api-openapi.yml
  format: yaml
  label: Meltwater Bring Your Own Content (BYOC) API
  slug: meltwater-bring-your-own-content-byoc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-bring-your-own-content-byoc-api-openapi.yml
- filename: meltwater-explore-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Analytics API
  slug: meltwater-explore-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-analytics-api-openapi.yml
- filename: meltwater-explore-assets-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Assets API
  slug: meltwater-explore-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-assets-api-openapi.yml
- filename: meltwater-explore-search-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Search API
  slug: meltwater-explore-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-search-api-openapi.yml
- filename: meltwater-listening-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Listening Analytics API
  slug: meltwater-listening-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-analytics-api-openapi.yml
- filename: meltwater-listening-exports-api-openapi.yml
  format: yaml
  label: Meltwater Listening Exports API
  slug: meltwater-listening-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-exports-api-openapi.yml
- filename: meltwater-listening-search-api-openapi.yml
  format: yaml
  label: Meltwater Listening Search API
  slug: meltwater-listening-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-search-api-openapi.yml
- filename: meltwater-listening-search-management-api-openapi.yml
  format: yaml
  label: Meltwater Listening Search Management API
  slug: meltwater-listening-search-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-search-management-api-openapi.yml
- filename: meltwater-listening-streaming-api-openapi.yml
  format: yaml
  label: Meltwater Listening Streaming API
  slug: meltwater-listening-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-streaming-api-openapi.yml
- filename: meltwater-mira-api-api-openapi.yml
  format: yaml
  label: Meltwater Mira API API
  slug: meltwater-mira-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-mira-api-api-openapi.yml
- filename: meltwater-owned-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Owned Analytics API
  slug: meltwater-owned-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-owned-analytics-api-openapi.yml
- filename: meltwater-api-v4-openapi.yml
  format: yaml
  label: Meltwater API v4
  slug: meltwater-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-api-v4-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Meltwater Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Meltwater secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Meltwater
provider_slug: meltwater
scheme_count: 2
schemes:
- description: All REST calls authenticate with a Meltwater API token sent in an `apikey` request header. HTTPS is mandatory - plain HTTP calls fail, and unauthenticated calls fail.
  in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/_original/meltwater-api-openapi.yaml
  - openapi/meltwater-api-v4-openapi.yml
  - https://developer.meltwater.com/api-reference/api-reference-overview
  type: apiKey
- applies_to: https://api.meltwater.com/v2/mcp
  dynamic_client_registration: https://app.meltwater.com/oauth/register
  flows:
  - authorizationUrl: https://app.meltwater.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    scopes:
    - tools:read
    - tools:call
    - openid
    - profile
    - email
    tokenUrl: https://app.meltwater.com/oauth/token
  name: oauth2
  sources:
  - https://api.meltwater.com/.well-known/oauth-protected-resource
  - https://app.meltwater.com/.well-known/oauth-authorization-server
  type: oauth2
slug: meltwater-authentication
source_filename: meltwater-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.meltwater.com/api-reference/api-reference-overview\ndocs:\n  - https://developer.meltwater.com/api-reference/api-reference-overview\n  - https://developer.meltwater.com/guides/getting-started/api-credentials\n  - https://developer.meltwater.com/guides/meltwater-mcp/connecting\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    The REST API is API-token only. OAuth 2.0 exists today only in front of the Meltwater MCP\n    server and is not declared in any OpenAPI - it was found in Meltwater's live RFC 9728 /\n    RFC 8414 discovery documents.\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: >-\n    All REST calls authenticate with a Meltwater API token sent in an `apikey` request header.\n    HTTPS is mandatory - plain HTTP calls fail, and unauthenticated calls fail.\n  sources:\n  - openapi/_original/meltwater-api-openapi.yaml\n\
  \  - openapi/meltwater-api-v4-openapi.yml\n  - https://developer.meltwater.com/api-reference/api-reference-overview\n- name: oauth2\n  type: oauth2\n  applies_to: https://api.meltwater.com/v2/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.meltwater.com/oauth/authorize\n    tokenUrl: https://app.meltwater.com/oauth/token\n    pkce: [S256]\n    scopes: [tools:read, tools:call, openid, profile, email]\n  dynamic_client_registration: https://app.meltwater.com/oauth/register\n  sources:\n  - https://api.meltwater.com/.well-known/oauth-protected-resource\n  - https://app.meltwater.com/.well-known/oauth-authorization-server\ntoken_management:\n  console: Account > Meltwater API in the Meltwater application\n  create: Create Token; the token value is shown once and cannot be retrieved later\n  revoke: Revoke button invalidates the token immediately\n  usage: per-token usage is visible in the app and via the `token_id` query parameter on the usage endpoints\n  permission_required:\
  \ Admin level access on the Meltwater API permission\n  docs: https://developer.meltwater.com/guides/getting-started/api-credentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/authentication/meltwater-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Media Monitoring
- Social Listening
- PR Analytics
- Brand Intelligence
- News API
- Social Analytics
- Media Intelligence
---
