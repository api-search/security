---
anonymous_access: false
api_key_in: []
api_specs:
- filename: organizewith-ai-assets-api-openapi.yml
  format: yaml
  label: Organize with AI Assets API
  slug: organizewith-ai-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/organizewith-ai/openapi/organizewith-ai-assets-api-openapi.yml
- filename: organizewith-ai-health-api-openapi.yml
  format: yaml
  label: Organize with AI Health API
  slug: organizewith-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/organizewith-ai/openapi/organizewith-ai-health-api-openapi.yml
- filename: organizewith-ai-mcp-api-openapi.yml
  format: yaml
  label: Organize with AI MCP API
  slug: organizewith-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/organizewith-ai/openapi/organizewith-ai-mcp-api-openapi.yml
- filename: organizewith-ai-well-known-api-openapi.yml
  format: yaml
  label: Organize with AI .well Known API
  slug: organizewith-ai-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/organizewith-ai/openapi/organizewith-ai-well-known-api-openapi.yml
auth_types: []
description: Organize with AI uses OAuth 2.0 Authorization Code flow with PKCE for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Organize with AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Organize with AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Organize with AI
provider_slug: organizewith-ai
scheme_count: 1
schemes:
- authorize_url: https://index.organizewith.ai/oauth/authorize
  evidence: OwAI supports OAuth dynamic client registration followed by user sign-in and consent using Authorization Code with PKCE (S256).
  flows:
  - authorization_code
  how_to_obtain: Register a client at https://index.organizewith.ai/oauth/register (dynamic client registration) and then perform the Authorization Code with PKCE flow to obtain an access token.
  name: OAuth
  scopes:
  - media:search
  - media:read
  - library:read
  - library:write
  - library:delete
  - ACCESS_VIEW_MANAGE_MCP_CONTENT
  - SHARE_THROUGH_MCP_CONVERSATION_INFO
  type: oauth2
slug: organizewith-ai-authentication
source_filename: organizewith-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://organizewith.ai/auth.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://organizewith.ai/auth.md\nsources:\n- https://organizewith.ai/auth.md\n- https://organizewith.ai/.well-known/oauth-protected-resource\n- https://organizewith.ai/en/guides/choose-your-owai-setup/index.md\n- https://organizewith.ai/en/guides/cli-getting-started/index.md\ndescription: Organize with AI uses OAuth 2.0 Authorization Code flow with PKCE for authentication.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: OwAI supports OAuth dynamic client registration followed by user sign-in and consent using Authorization Code with PKCE (S256).\n  flows:\n  - authorization_code\n  authorize_url: https://index.organizewith.ai/oauth/authorize\n  scopes:\n  - media:search\n  - media:read\n  - library:read\n  - library:write\n  - library:delete\n  - ACCESS_VIEW_MANAGE_MCP_CONTENT\n  - SHARE_THROUGH_MCP_CONVERSATION_INFO\n  how_to_obtain: Register a client at https://index.organizewith.ai/oauth/register\
  \ (dynamic client registration) and then perform the Authorization\n    Code with PKCE flow to obtain an access token.\ndocs: https://organizewith.ai/auth.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/organizewith-ai/authentication/organizewith-ai-authentication.yml
summary_line: 1 scheme
tags:
- Photo Organization
- video organization
- AI Search
- cloud indexing
- MCP integration
- OneDrive integration
- Apple Photos integration
---
