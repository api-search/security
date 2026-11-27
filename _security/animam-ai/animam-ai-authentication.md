---
anonymous_access: false
api_key_in: []
api_specs:
- filename: animam-ai-corpus-api-openapi.yml
  format: yaml
  label: Animam.ai Corpus API
  slug: animam-ai-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-corpus-api-openapi.yml
- filename: animam-ai-segments-api-openapi.yml
  format: yaml
  label: Animam.ai Segments API
  slug: animam-ai-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-segments-api-openapi.yml
- filename: animam-ai-tenants-api-openapi.yml
  format: yaml
  label: Animam.ai Tenants API
  slug: animam-ai-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-tenants-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Animam.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Animam.ai declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Animam.ai
provider_slug: animam-ai
scheme_count: 3
schemes:
- bearerFormat: API key (ak_...) or JWT
  description: 'Static API key (`Authorization: Bearer ak_xxx`) or short-lived JWT issued by /oauth/token.'
  scheme: bearer
  type: http
- description: Alternative header for legacy integrations.
  in: header
  name: X-API-Key
  type: apiKey
- description: OAuth 2.1 + PKCE for MCP-style agent integrations.
  flows:
    authorizationCode:
      authorizationUrl: https://api.animam.ai/oauth/authorize
      scopes:
        corpus:read: Read knowledge base entries
        corpus:write: Create / update / delete knowledge base entries
        segments:read: Read segments
        segments:write: Create / update segments
        settings:read: Read tenant settings
        settings:write: Update tenant settings
        stats:read: Read analytics and usage data
      tokenUrl: https://api.animam.ai/oauth/token
  type: oauth2
slug: animam-ai-authentication
source_filename: animam-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://api.animam.ai/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Static API key (`Authorization: Bearer ak_xxx`) or short-lived JWT issued by /oauth/token.\"\n    bearerFormat: \"API key (ak_...) or JWT\"\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: \"Alternative header for legacy integrations.\"\n  - type: oauth2\n    description: \"OAuth 2.1 + PKCE for MCP-style agent integrations.\"\n    flows:\n      authorizationCode:\n        authorizationUrl: \"https://api.animam.ai/oauth/authorize\"\n        tokenUrl: \"https://api.animam.ai/oauth/token\"\n        scopes:\n          corpus:read: \"Read knowledge base entries\"\n          corpus:write: \"Create / update / delete knowledge base entries\"\n          segments:read: \"Read segments\"\n          segments:write: \"Create / update segments\"\n          settings:read: \"Read tenant settings\"\n          settings:write:\
  \ \"Update tenant settings\"\n          stats:read: \"Read analytics and usage data\"\n"
source_yaml_url: https://artifacts.apis.io/animam-ai/authentication/animam-ai-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Automation
- Lead Generation
- Chatbots
- Software-as-a-Service
---
