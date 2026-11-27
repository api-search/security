---
anonymous_access: false
api_key_in: []
api_specs:
- filename: breakreach-com-accounts-api-openapi.yml
  format: yaml
  label: Breakreach Accounts API
  slug: breakreach-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-accounts-api-openapi.yml
- filename: breakreach-com-analytics-api-openapi.yml
  format: yaml
  label: Breakreach Analytics API
  slug: breakreach-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-analytics-api-openapi.yml
- filename: breakreach-com-comment-dm-rules-api-openapi.yml
  format: yaml
  label: Breakreach Comment Dm Rules API
  slug: breakreach-com-comment-dm-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-comment-dm-rules-api-openapi.yml
- filename: breakreach-com-comments-api-openapi.yml
  format: yaml
  label: Breakreach Comments API
  slug: breakreach-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-comments-api-openapi.yml
- filename: breakreach-com-connect-links-api-openapi.yml
  format: yaml
  label: Breakreach Connect Links API
  slug: breakreach-com-connect-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-connect-links-api-openapi.yml
- filename: breakreach-com-dm-automations-api-openapi.yml
  format: yaml
  label: Breakreach Dm Automations API
  slug: breakreach-com-dm-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-dm-automations-api-openapi.yml
- filename: breakreach-com-inbox-api-openapi.yml
  format: yaml
  label: Breakreach Inbox API
  slug: breakreach-com-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-inbox-api-openapi.yml
- filename: breakreach-com-media-api-openapi.yml
  format: yaml
  label: Breakreach Media API
  slug: breakreach-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-media-api-openapi.yml
- filename: breakreach-com-next-slot-api-openapi.yml
  format: yaml
  label: Breakreach Next Slot API
  slug: breakreach-com-next-slot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-next-slot-api-openapi.yml
- filename: breakreach-com-performance-api-openapi.yml
  format: yaml
  label: Breakreach Performance API
  slug: breakreach-com-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-performance-api-openapi.yml
- filename: breakreach-com-pinterest-boards-api-openapi.yml
  format: yaml
  label: Breakreach Pinterest Boards API
  slug: breakreach-com-pinterest-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-pinterest-boards-api-openapi.yml
- filename: breakreach-com-post-insights-api-openapi.yml
  format: yaml
  label: Breakreach Post Insights API
  slug: breakreach-com-post-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-post-insights-api-openapi.yml
- filename: breakreach-com-posts-api-openapi.yml
  format: yaml
  label: Breakreach Posts API
  slug: breakreach-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-posts-api-openapi.yml
- filename: breakreach-com-workspaces-api-openapi.yml
  format: yaml
  label: Breakreach Workspaces API
  slug: breakreach-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breakreach-com/openapi/breakreach-com-workspaces-api-openapi.yml
auth_types: []
description: 'Breakreach supports two authentication methods for its MCP servers: an API key sent as a Bearer token, and OAuth 2.0 for services like Bluesky that require it.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Breakreach Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breakreach declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Breakreach
provider_slug: breakreach-com
scheme_count: 2
schemes:
- evidence: Clients that handle OAuth sign you in; others send an API key from Settings → API & MCP.
  header: Authorization
  how_to_obtain: Generate an API key in Breakreach Settings → API & MCP and include it as a Bearer token.
  location: header
  name: Breakreach API key
  type: http-bearer
- evidence: 'Breakreach does: you authorize it on Bluesky''s page from Claude''s or ChatGPT''s directory, and posts go out from our servers at the time you set.'
  how_to_obtain: Authorize Breakreach on Bluesky’s OAuth page via the connector UI (Claude, ChatGPT, or Breakreach’s web UI).
  name: Bluesky OAuth
  type: oauth2
slug: breakreach-com-authentication
source_filename: breakreach-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.breakreach.com/mcp/bluesky
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.breakreach.com/mcp/bluesky\nsources:\n- https://www.breakreach.com/mcp/bluesky\n- https://www.breakreach.com/developers/bluesky-api\n- https://www.breakreach.com/developers/devto-api\n- https://www.breakreach.com/developers/tumblr-api\ndescription: 'Breakreach supports two authentication methods for its MCP servers: an API key sent as a Bearer token, and OAuth 2.0 for services\n  like Bluesky that require it.'\nschemes:\n- type: http-bearer\n  name: Breakreach API key\n  evidence: Clients that handle OAuth sign you in; others send an API key from Settings → API & MCP.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in Breakreach Settings → API & MCP and include it as a Bearer token.\n- type: oauth2\n  name: Bluesky OAuth\n  evidence: 'Breakreach does: you authorize it on Bluesky''s page from Claude''s or ChatGPT''s directory, and posts\
  \ go out from our servers at\n    the time you set.'\n  how_to_obtain: Authorize Breakreach on Bluesky’s OAuth page via the connector UI (Claude, ChatGPT, or Breakreach’s web UI).\ndocs: https://www.breakreach.com/mcp/bluesky\n"
source_yaml_url: https://artifacts.apis.io/breakreach-com/authentication/breakreach-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Social Media
- Automation
- Scheduling
- Marketing
---
