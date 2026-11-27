---
anonymous_access: false
api_key_in: []
api_specs:
- filename: annsa-ai-agents-api-openapi.yml
  format: yaml
  label: Annsa Agents API
  slug: annsa-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-agents-api-openapi.yml
- filename: annsa-ai-ingest-api-openapi.yml
  format: yaml
  label: Annsa Ingest API
  slug: annsa-ai-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-ingest-api-openapi.yml
- filename: annsa-ai-service-api-openapi.yml
  format: yaml
  label: Annsa Service API
  slug: annsa-ai-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-service-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Annsa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Annsa declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Annsa
provider_slug: annsa-ai
scheme_count: 3
schemes:
- description: OAuth 2.0 with PKCE for MCP resource
  flows:
    authorizationCode:
      authorizationUrl: https://app.annsa.ai/mcp/auth
      scopes:
        read: Read priorities, specs, survey results and search.
        write: Change state — start building, mark shipped, share back with customers.
      tokenUrl: https://app.annsa.ai/mcp/token
  type: oauth2
- bearerFormat: JWT
  description: Supabase session token for signed-in user
  type: bearer
- description: Survey key used in WidgetSubmission schema
  in: body
  name: api_key
  type: apiKey
slug: annsa-ai-authentication
source_filename: annsa-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: \"https://annsa.ai/auth.md\"\nschemes:\n  - type: oauth2\n    description: \"OAuth 2.0 with PKCE for MCP resource\"\n    flows:\n      authorizationCode:\n        authorizationUrl: \"https://app.annsa.ai/mcp/auth\"\n        tokenUrl: \"https://app.annsa.ai/mcp/token\"\n        scopes:\n          read: \"Read priorities, specs, survey results and search.\"\n          write: \"Change state — start building, mark shipped, share back with customers.\"\n  - type: bearer\n    description: \"Supabase session token for signed-in user\"\n    bearerFormat: \"JWT\"\n  - type: apiKey\n    name: api_key\n    in: body\n    description: \"Survey key used in WidgetSubmission schema\"\n"
source_yaml_url: https://artifacts.apis.io/annsa-ai/authentication/annsa-ai-authentication.yml
summary_line: 3 schemes
tags:
- Project Management
- Customer Management
- Agent Teams
- Artificial Intelligence
- Software-as-a-Service
---
