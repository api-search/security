---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fluxaipro-art-agent-integration-api-openapi.yml
  format: yaml
  label: Flux AI Agent Integration API
  slug: fluxaipro-art-agent-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxaipro-art/openapi/fluxaipro-art-agent-integration-api-openapi.yml
- filename: fluxaipro-art-ai-generations-api-openapi.yml
  format: yaml
  label: Flux AI AI Generations API
  slug: fluxaipro-art-ai-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxaipro-art/openapi/fluxaipro-art-ai-generations-api-openapi.yml
- filename: fluxaipro-art-models-api-openapi.yml
  format: yaml
  label: Flux AI Models API
  slug: fluxaipro-art-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxaipro-art/openapi/fluxaipro-art-models-api-openapi.yml
auth_types: []
description: Authentication methods for Flux AI MCP and REST API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Flux AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flux AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Flux AI
provider_slug: fluxaipro-art
scheme_count: 2
schemes:
- evidence: The first connection opens a Flux AI sign-in and consent screen (OAuth 2.1 with PKCE).
  header: Authorization
  how_to_obtain: User signs in via browser; consent screen grants scopes; token is issued for resource https://fluxaipro.art/api/mcp
  location: header
  name: Flux AI OAuth
  scopes:
  - mcp:read
  - mcp:generate
  - mcp:upload
  type: oauth2
- evidence: MCP also accepts a dashboard API key as a bearer token
  header: Authorization
  how_to_obtain: Sign in, open API keys in your dashboard and create a key
  location: header
  name: Dashboard API key
  type: apiKey
slug: fluxaipro-art-authentication
source_filename: fluxaipro-art-authentication.yml
source_heading: Authentication Profile
source_url: https://fluxaipro.art/docs/mcp/credits-and-security
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fluxaipro.art/docs/mcp/credits-and-security\nsources:\n- https://fluxaipro.art/docs/mcp/credits-and-security\n- https://fluxaipro.art/docs/mcp/rest-api\n- https://fluxaipro.art/mcp\n- https://fluxaipro.art/de/mcp\ndescription: Authentication methods for Flux AI MCP and REST API\nschemes:\n- type: oauth2\n  name: Flux AI OAuth\n  evidence: The first connection opens a Flux AI sign-in and consent screen (OAuth 2.1 with PKCE).\n  location: header\n  header: Authorization\n  scopes:\n  - mcp:read\n  - mcp:generate\n  - mcp:upload\n  how_to_obtain: User signs in via browser; consent screen grants scopes; token is issued for resource https://fluxaipro.art/api/mcp\n- type: apiKey\n  name: Dashboard API key\n  evidence: MCP also accepts a dashboard API key as a bearer token\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in, open API keys in your dashboard and\
  \ create a key\ndocs: https://fluxaipro.art/docs/mcp/credits-and-security\n"
source_yaml_url: https://artifacts.apis.io/fluxaipro-art/authentication/fluxaipro-art-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Image Generation
- Creative Tools
- Prompt Engineering
- Company
---
