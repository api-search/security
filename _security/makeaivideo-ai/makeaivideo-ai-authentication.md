---
anonymous_access: false
api_key_in: []
api_specs:
- filename: makeaivideo-ai-auth-api-openapi.yml
  format: yaml
  label: MakeAIVideo Auth API
  slug: makeaivideo-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-auth-api-openapi.yml
- filename: makeaivideo-ai-brand-kit-api-openapi.yml
  format: yaml
  label: MakeAIVideo Brand kit API
  slug: makeaivideo-ai-brand-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-brand-kit-api-openapi.yml
- filename: makeaivideo-ai-characters-api-openapi.yml
  format: yaml
  label: MakeAIVideo Characters API
  slug: makeaivideo-ai-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-characters-api-openapi.yml
- filename: makeaivideo-ai-ideas-api-openapi.yml
  format: yaml
  label: MakeAIVideo Ideas API
  slug: makeaivideo-ai-ideas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-ideas-api-openapi.yml
- filename: makeaivideo-ai-introspection-api-openapi.yml
  format: yaml
  label: MakeAIVideo Introspection API
  slug: makeaivideo-ai-introspection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-introspection-api-openapi.yml
- filename: makeaivideo-ai-music-api-openapi.yml
  format: yaml
  label: MakeAIVideo Music API
  slug: makeaivideo-ai-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-music-api-openapi.yml
- filename: makeaivideo-ai-publishing-api-openapi.yml
  format: yaml
  label: MakeAIVideo Publishing API
  slug: makeaivideo-ai-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-publishing-api-openapi.yml
- filename: makeaivideo-ai-scripts-api-openapi.yml
  format: yaml
  label: MakeAIVideo Scripts API
  slug: makeaivideo-ai-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-scripts-api-openapi.yml
- filename: makeaivideo-ai-uploads-api-openapi.yml
  format: yaml
  label: MakeAIVideo Uploads API
  slug: makeaivideo-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-uploads-api-openapi.yml
- filename: makeaivideo-ai-videos-api-openapi.yml
  format: yaml
  label: MakeAIVideo Videos API
  slug: makeaivideo-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-videos-api-openapi.yml
- filename: makeaivideo-ai-voices-api-openapi.yml
  format: yaml
  label: MakeAIVideo Voices API
  slug: makeaivideo-ai-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-voices-api-openapi.yml
- filename: makeaivideo-ai-webhooks-api-openapi.yml
  format: yaml
  label: MakeAIVideo Webhooks API
  slug: makeaivideo-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-webhooks-api-openapi.yml
- filename: makeaivideo-ai-workspace-api-openapi.yml
  format: yaml
  label: MakeAIVideo Workspace API
  slug: makeaivideo-ai-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-workspace-api-openapi.yml
auth_types: []
description: Authentication methods for MakeAIVideo API and MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MakeAIVideo Authentication
name_suffix: Authentication
oauth_flows: []
overview: MakeAIVideo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MakeAIVideo
provider_slug: makeaivideo-ai
scheme_count: 2
schemes:
- evidence: Every endpoint except the device-login pair takes an organization API key as a bearer token.
  header: Authorization
  how_to_obtain: Create a key in the app under Settings → Advanced → API keys; keys are prefixed mav_ and belong to an organization.
  location: header
  name: Bearer
  scopes:
  - read
  - write
  - ai
  type: http-bearer
- authorize_url: https://app.makeaivideo.ai/api/v1/auth/device
  evidence: 'Authentication is required: either OAuth, which most clients handle for you, or an Authorization: Bearer mav_... header.'
  header: Authorization
  how_to_obtain: 'Use the device‑code flow (RFC 8628): POST /auth/device to get a user code, have the user approve it, then poll POST /auth/device/token to receive the API key.'
  location: header
  name: OAuth2 Device Code
  scopes:
  - read
  - write
  - ai
  token_url: https://app.makeaivideo.ai/api/v1/auth/device/token
  type: oauth2
slug: makeaivideo-ai-authentication
source_filename: makeaivideo-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://makeaivideo.ai/docs/authentication
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://makeaivideo.ai/docs/authentication\nsources:\n- https://makeaivideo.ai/docs/authentication\n- https://makeaivideo.ai/docs/mcp\n- https://makeaivideo.ai/docs/quickstart\n- https://makeaivideo.ai/docs/api/auth\ndescription: Authentication methods for MakeAIVideo API and MCP server\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every endpoint except the device-login pair takes an organization API key as a bearer token.\n  location: header\n  header: Authorization\n  scopes:\n  - read\n  - write\n  - ai\n  how_to_obtain: Create a key in the app under Settings → Advanced → API keys; keys are prefixed mav_ and belong to an organization.\n- type: oauth2\n  name: OAuth2 Device Code\n  evidence: 'Authentication is required: either OAuth, which most clients handle for you, or an Authorization: Bearer mav_... header.'\n  location: header\n  header: Authorization\n  token_url:\
  \ https://app.makeaivideo.ai/api/v1/auth/device/token\n  authorize_url: https://app.makeaivideo.ai/api/v1/auth/device\n  scopes:\n  - read\n  - write\n  - ai\n  how_to_obtain: 'Use the device‑code flow (RFC 8628): POST /auth/device to get a user code, have the user approve it, then poll POST /auth/device/token\n    to receive the API key.'\ndocs: https://makeaivideo.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/makeaivideo-ai/authentication/makeaivideo-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI Video Generation
- Social Media Content
- Advertising
- Developer API
---
