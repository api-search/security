---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deploy-social-account-api-openapi.yml
  format: yaml
  label: deploy.social Account API
  slug: deploy-social-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deploy-social/openapi/deploy-social-account-api-openapi.yml
- filename: deploy-social-destinations-api-openapi.yml
  format: yaml
  label: deploy.social Destinations API
  slug: deploy-social-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deploy-social/openapi/deploy-social-destinations-api-openapi.yml
- filename: deploy-social-media-api-openapi.yml
  format: yaml
  label: deploy.social Media API
  slug: deploy-social-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deploy-social/openapi/deploy-social-media-api-openapi.yml
- filename: deploy-social-posts-api-openapi.yml
  format: yaml
  label: deploy.social Posts API
  slug: deploy-social-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deploy-social/openapi/deploy-social-posts-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Deploy Social Authentication
name_suffix: Authentication
oauth_flows: []
overview: deploy.social secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: deploy.social
provider_slug: deploy-social
scheme_count: 2
schemes:
- access_levels:
  - read
  - read and write
  availability: Standard and Studio plans only
  description: Your API key, from the API tab in Deploy. Keys start with `ds_live_`.
  docs_text: Open Account → API in Deploy and create a key for one workspace. Choose read access to look things up, or read and write access to add media and posts. A key acts as the member who created it, within that workspace.
  header: 'Authorization: Bearer <key>'
  key_prefix: ds_live_
  name: apiKey
  scheme: bearer
  sources:
  - openapi/deploy-social-openapi.yml
  - https://deploy.social/docs/api
  type: http
- description: Claude.ai and ChatGPT connect to the remote MCP server (https://api.deploy.social/mcp) with an OAuth sign-in to Deploy, then pick one workspace and choose read-only or read and write access. Claude Code, Cursor and VS Code use a workspace API key as a Bearer token instead. Applies to the MCP server, not the REST contract.
  name: mcp-oauth
  sources:
  - https://deploy.social/docs/mcp
  type: oauth2
slug: deploy-social-authentication
source_filename: deploy-social-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://deploy.social/docs/api\ndocs: https://deploy.social/docs/api\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Your API key, from the API tab in Deploy. Keys start with `ds_live_`.\n  key_prefix: ds_live_\n  header: 'Authorization: Bearer <key>'\n  docs_text: Open Account → API in Deploy and create a key for one workspace. Choose read access to look things\n    up, or read and write access to add media and posts. A key acts as the member who created it, within that\n    workspace.\n  access_levels:\n  - read\n  - read and write\n  availability: Standard and Studio plans only\n  sources:\n  - openapi/deploy-social-openapi.yml\n  - https://deploy.social/docs/api\n- name: mcp-oauth\n  type: oauth2\n  description: Claude.ai and ChatGPT connect to the remote MCP server (https://api.deploy.social/mcp) with an\n    OAuth sign-in to Deploy, then pick one workspace\
  \ and choose read-only or read and write access. Claude Code,\n    Cursor and VS Code use a workspace API key as a Bearer token instead. Applies to the MCP server, not the\n    REST contract.\n  sources:\n  - https://deploy.social/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/deploy-social/authentication/deploy-social-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Social Media
- Video
- Short-Form Video
- Cross-Posting
- Scheduling
- Content Publishing
- MCP
---
