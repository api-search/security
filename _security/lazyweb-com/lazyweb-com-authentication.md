---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lazyweb-com-antigravity-md-api-openapi.yml
  format: yaml
  label: lazyweb-com Antigravity.md API
  slug: lazyweb-com-antigravity-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-antigravity-md-api-openapi.yml
- filename: lazyweb-com-chatgpt-md-api-openapi.yml
  format: yaml
  label: lazyweb-com Chatgpt.md API
  slug: lazyweb-com-chatgpt-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-chatgpt-md-api-openapi.yml
- filename: lazyweb-com-claude-md-api-openapi.yml
  format: yaml
  label: lazyweb-com Claude.md API
  slug: lazyweb-com-claude-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-claude-md-api-openapi.yml
- filename: lazyweb-com-codex-md-api-openapi.yml
  format: yaml
  label: lazyweb-com Codex.md API
  slug: lazyweb-com-codex-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-codex-md-api-openapi.yml
- filename: lazyweb-com-cursor-md-api-openapi.yml
  format: yaml
  label: lazyweb-com Cursor.md API
  slug: lazyweb-com-cursor-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-cursor-md-api-openapi.yml
- filename: lazyweb-com-index-md-api-openapi.yml
  format: yaml
  label: lazyweb-com Index.md API
  slug: lazyweb-com-index-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-index-md-api-openapi.yml
- filename: lazyweb-com-install-sh-api-openapi.yml
  format: yaml
  label: lazyweb-com Install.sh API
  slug: lazyweb-com-install-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-install-sh-api-openapi.yml
- filename: lazyweb-com-mcp-api-openapi.yml
  format: yaml
  label: lazyweb-com MCP API
  slug: lazyweb-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-mcp-api-openapi.yml
- filename: lazyweb-com-pricing-md-api-openapi.yml
  format: yaml
  label: lazyweb-com Pricing.md API
  slug: lazyweb-com-pricing-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-pricing-md-api-openapi.yml
- filename: lazyweb-com-use-lazyweb-md-api-openapi.yml
  format: yaml
  label: lazyweb-com Use Lazyweb.md API
  slug: lazyweb-com-use-lazyweb-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-use-lazyweb-md-api-openapi.yml
- filename: lazyweb-com-well-known-api-openapi.yml
  format: yaml
  label: lazyweb-com .well Known API
  slug: lazyweb-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyweb-com/openapi/lazyweb-com-well-known-api-openapi.yml
auth_types: []
description: Authentication methods for Lazyweb as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lazyweb Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: lazyweb-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: lazyweb-com
provider_slug: lazyweb-com
scheme_count: 2
schemes:
- evidence: 'The header-based `https://www.lazyweb.com/mcp` bearer path remains for clients that send `Authorization: Bearer <token>` (Claude Code, Cursor, Codex, Antigravity).'
  header: Authorization
  how_to_obtain: Create or reuse a bearer token via the installer; token is read from LAZYWEB_MCP_TOKEN, ~/.lazyweb/lazyweb_mcp_token, or https://www.lazyweb.com/api/mcp/install-token.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Claude.ai, Claude Desktop, and Claude Mobile connect through a remote MCP connector and authenticate it with OAuth — there is no field to paste an Authorization header. Lazyweb runs a standard OAuth 2.1 authorization server (PKCE + Dynamic Client Registration) on the `/mcp` resource.
  how_to_obtain: Sign in with email and a 6‑digit verification code; the connector performs dynamic client registration and PKCE flow automatically.
  name: Lazyweb OAuth
  type: oauth2
slug: lazyweb-com-authentication
source_filename: lazyweb-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.lazyweb.com/claude.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.lazyweb.com/claude.md\nsources:\n- https://www.lazyweb.com/claude.md\n- https://www.lazyweb.com/cursor.md\n- https://www.lazyweb.com/codex.md\n- https://www.lazyweb.com/antigravity.md\ndescription: Authentication methods for Lazyweb as documented\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'The header-based `https://www.lazyweb.com/mcp` bearer path remains for clients that send `Authorization: Bearer <token>` (Claude\n    Code, Cursor, Codex, Antigravity).'\n  location: header\n  header: Authorization\n  how_to_obtain: Create or reuse a bearer token via the installer; token is read from LAZYWEB_MCP_TOKEN, ~/.lazyweb/lazyweb_mcp_token, or https://www.lazyweb.com/api/mcp/install-token.\n- type: oauth2\n  name: Lazyweb OAuth\n  evidence: Claude.ai, Claude Desktop, and Claude Mobile connect through a remote MCP connector and authenticate it with OAuth\
  \ — there is no field\n    to paste an Authorization header. Lazyweb runs a standard OAuth 2.1 authorization server (PKCE + Dynamic Client Registration) on the `/mcp`\n    resource.\n  how_to_obtain: Sign in with email and a 6‑digit verification code; the connector performs dynamic client registration and PKCE flow automatically.\ndocs: https://www.lazyweb.com/claude.md\n"
source_yaml_url: https://artifacts.apis.io/lazyweb-com/authentication/lazyweb-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- SaaS
- Growth
- AI
- No-code
---
