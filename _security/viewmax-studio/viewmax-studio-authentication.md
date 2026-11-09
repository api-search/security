---
anonymous_access: false
api_key_in: []
api_specs:
- filename: viewmax-studio-account-api-openapi.yml
  format: yaml
  label: ViewMax Studio Account API
  slug: viewmax-studio-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-account-api-openapi.yml
- filename: viewmax-studio-advanced-api-openapi.yml
  format: yaml
  label: ViewMax Studio Advanced API
  slug: viewmax-studio-advanced-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-advanced-api-openapi.yml
- filename: viewmax-studio-catalog-api-openapi.yml
  format: yaml
  label: ViewMax Studio Catalog API
  slug: viewmax-studio-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-catalog-api-openapi.yml
- filename: viewmax-studio-generation-api-openapi.yml
  format: yaml
  label: ViewMax Studio Generation API
  slug: viewmax-studio-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-generation-api-openapi.yml
- filename: viewmax-studio-tasks-api-openapi.yml
  format: yaml
  label: ViewMax Studio Tasks API
  slug: viewmax-studio-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-tasks-api-openapi.yml
auth_types: []
description: Authentication methods for ViewMax Studio APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Viewmax Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: ViewMax Studio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ViewMax Studio
provider_slug: viewmax-studio
scheme_count: 2
schemes:
- evidence: 'Send the key in the Authorization header on every authenticated request: Authorization : Bearer sk-your-api-key'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys and store it in a secret manager or environment variable such as VIEWMAX_API_KEY.
  location: header
  name: API Key
  type: http-bearer
- evidence: OAuth (claude.ai and Claude Desktop). Add a custom connector with the URL above, click Connect, and sign in with your ViewMax account. Clients discover the flow through /.well-known/oauth-protected-resource ; no API key is needed.
  how_to_obtain: Sign in with your ViewMax account via the connector; the flow is discovered through /.well-known/oauth-protected-resource.
  name: MCP OAuth
  type: oauth2
slug: viewmax-studio-authentication
source_filename: viewmax-studio-authentication.yml
source_heading: Authentication Profile
source_url: https://viewmax.studio/docs/api/authentication
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://viewmax.studio/docs/api/authentication\nsources:\n- https://viewmax.studio/docs/api/authentication\n- https://viewmax.studio/docs/api/authentication\n- https://viewmax.studio/docs/mcp\n- https://viewmax.studio/docs/api\ndescription: Authentication methods for ViewMax Studio APIs\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send the key in the Authorization header on every authenticated request: Authorization : Bearer sk-your-api-key'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys and store it in a secret manager or environment variable such as VIEWMAX_API_KEY.\n- type: oauth2\n  name: MCP OAuth\n  evidence: OAuth (claude.ai and Claude Desktop). Add a custom connector with the URL above, click Connect, and sign in with your ViewMax account.\n    Clients discover the flow through /.well-known/oauth-protected-resource\
  \ ; no API key is needed.\n  how_to_obtain: Sign in with your ViewMax account via the connector; the flow is discovered through /.well-known/oauth-protected-resource.\ndocs: https://viewmax.studio/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/viewmax-studio/authentication/viewmax-studio-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Video
- Generation
- Marketing
---
