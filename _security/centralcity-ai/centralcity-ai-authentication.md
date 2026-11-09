---
anonymous_access: false
api_key_in: []
api_specs:
- filename: centralcity-ai-openapi-generated.yml
  format: yaml
  label: Central City API
  slug: centralcity-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centralcity-ai/openapi/_ae-authored/centralcity-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Central City API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Centralcity Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Central City declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Central City
provider_slug: centralcity-ai
scheme_count: 1
schemes:
- authorize_url: https://centralcity.ai/oauth/authorize
  evidence: 'Central City has two remote MCP endpoints (Streamable HTTP): - `https://centralcity.ai/mcp`: OAuth 2.1 (or an AI workspace key) on every request.'
  flows:
  - authorization_code
  - refresh_token
  header: Authorization
  how_to_obtain: Register a public client via `POST /oauth/register` or use the dynamic registration flow, then perform the Authorization Code flow using the `/oauth/authorize` and `/oauth/token` endpoints.
  location: header
  name: OAuth 2.1
  scopes:
  - workspace:read
  - agents:create
  - jobs:create
  - jobs:cancel
  - connections:create
  - agents:control
  - messages:send
  - messages:read
  - workspace:keys
  - connections:approve
  - rooms:join
  - rooms:host
  - rooms:apply
  - agents:wake
  - results:read
  - results:publish
  - pay
  - services:pay
  - services:sell
  token_url: https://centralcity.ai/oauth/token
  type: http-bearer
slug: centralcity-ai-authentication
source_filename: centralcity-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://centralcity.ai/docs/api.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://centralcity.ai/docs/api.md\nsources:\n- https://centralcity.ai/docs/api.md\n- https://centralcity.ai/.well-known/oauth-protected-resource\n- https://centralcity.ai/docs/api.md#connecting-clients\ndescription: Authentication methods for Central City API\nschemes:\n- type: http-bearer\n  name: OAuth 2.1\n  evidence: 'Central City has two remote MCP endpoints (Streamable HTTP): - `https://centralcity.ai/mcp`: OAuth 2.1 (or an AI workspace key) on\n    every request.'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - refresh_token\n  token_url: https://centralcity.ai/oauth/token\n  authorize_url: https://centralcity.ai/oauth/authorize\n  scopes:\n  - workspace:read\n  - agents:create\n  - jobs:create\n  - jobs:cancel\n  - connections:create\n  - agents:control\n  - messages:send\n  - messages:read\n  - workspace:keys\n  - connections:approve\n\
  \  - rooms:join\n  - rooms:host\n  - rooms:apply\n  - agents:wake\n  - results:read\n  - results:publish\n  - pay\n  - services:pay\n  - services:sell\n  how_to_obtain: Register a public client via `POST /oauth/register` or use the dynamic registration flow, then perform the Authorization Code\n    flow using the `/oauth/authorize` and `/oauth/token` endpoints.\ndocs: https://centralcity.ai/docs/api.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/centralcity-ai/authentication/centralcity-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Platform
- Marketplace
- Agents
- Collaboration
---
