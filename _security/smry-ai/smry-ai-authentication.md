---
anonymous_access: false
api_key_in: []
api_specs:
- filename: smry-ai-account-api-openapi.yml
  format: yaml
  label: smry-ai Account API
  slug: smry-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-account-api-openapi.yml
- filename: smry-ai-articles-api-openapi.yml
  format: yaml
  label: smry-ai Articles API
  slug: smry-ai-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-articles-api-openapi.yml
- filename: smry-ai-collections-api-openapi.yml
  format: yaml
  label: smry-ai Collections API
  slug: smry-ai-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-collections-api-openapi.yml
- filename: smry-ai-consumers-api-openapi.yml
  format: yaml
  label: smry-ai Consumers API
  slug: smry-ai-consumers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-consumers-api-openapi.yml
- filename: smry-ai-feeds-api-openapi.yml
  format: yaml
  label: smry-ai Feeds API
  slug: smry-ai-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-feeds-api-openapi.yml
- filename: smry-ai-library-api-openapi.yml
  format: yaml
  label: smry-ai Library API
  slug: smry-ai-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-library-api-openapi.yml
- filename: smry-ai-monitors-api-openapi.yml
  format: yaml
  label: smry-ai Monitors API
  slug: smry-ai-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-monitors-api-openapi.yml
- filename: smry-ai-public-reading-api-openapi.yml
  format: yaml
  label: smry-ai Public reading API
  slug: smry-ai-public-reading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-public-reading-api-openapi.yml
- filename: smry-ai-scouting-api-openapi.yml
  format: yaml
  label: smry-ai Scouting API
  slug: smry-ai-scouting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smry-ai/openapi/smry-ai-scouting-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Smry Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: smry-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: smry-ai
provider_slug: smry-ai
scheme_count: 2
schemes:
- description: Clerk OAuth with Authorization Code + PKCE for interactive clients.
  flows:
    authorizationCode:
      authorizationUrl: https://smry.ai/auth
      scopes:
        smry:read: Read‑only access to public and private resources.
        smry:write: Write access for mutations and MCP.
      tokenUrl: https://smry.ai/token
  type: oauth2
- description: Personal smry key for unattended clients.
  in: header
  name: X-API-Key
  type: apiKey
slug: smry-ai-authentication
source_filename: smry-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://smry.ai/auth.md\nname: smry-ai authentication\nschemes:\n  - type: oauth2\n    description: Clerk OAuth with Authorization Code + PKCE for interactive clients.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://smry.ai/auth\n        tokenUrl: https://smry.ai/token\n        scopes:\n          smry:read: Read‑only access to public and private resources.\n          smry:write: Write access for mutations and MCP.\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: Personal smry key for unattended clients.\n"
source_yaml_url: https://artifacts.apis.io/smry-ai/authentication/smry-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- News
- RSS
- Summarization
- Productivity
---
