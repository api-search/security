---
anonymous_access: false
api_key_in: []
api_specs:
- filename: audiomap-ai-ask-api-openapi.yml
  format: yaml
  label: AudioMap Ask API
  slug: audiomap-ai-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiomap-ai/openapi/audiomap-ai-ask-api-openapi.yml
- filename: audiomap-ai-content-api-openapi.yml
  format: yaml
  label: AudioMap Content API
  slug: audiomap-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiomap-ai/openapi/audiomap-ai-content-api-openapi.yml
- filename: audiomap-ai-deliverables-api-openapi.yml
  format: yaml
  label: AudioMap Deliverables API
  slug: audiomap-ai-deliverables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiomap-ai/openapi/audiomap-ai-deliverables-api-openapi.yml
- filename: audiomap-ai-notes-api-openapi.yml
  format: yaml
  label: AudioMap Notes API
  slug: audiomap-ai-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiomap-ai/openapi/audiomap-ai-notes-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AudioMap Authentication
name_suffix: Authentication
oauth_flows: []
overview: AudioMap declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AudioMap
provider_slug: audiomap-ai
scheme_count: 2
schemes:
- description: Bearer token for API access. Create API key at dashboard.
  example: Bearer am_live_...
  in: header
  name: Authorization
  type: apiKey
- description: OAuth 2.1 for MCP clients, supports PKCE, token TTL 1h, refresh 30d.
  flows:
    authorizationCode:
      authorizationUrl: https://api.audiomap.ai/.well-known/oauth-authorization-server
      scopes:
        read: Read access
        write: Write access
      tokenUrl: https://api.audiomap.ai/.well-known/oauth-protected-resource
  type: oauth2
slug: audiomap-ai-authentication
source_filename: audiomap-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: \"https://audiomap.ai/es/developers\"\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token for API access. Create API key at dashboard.\"\n    example: \"Bearer am_live_...\"\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: \"https://api.audiomap.ai/.well-known/oauth-authorization-server\"\n        tokenUrl: \"https://api.audiomap.ai/.well-known/oauth-protected-resource\"\n        scopes:\n          read: \"Read access\"\n          write: \"Write access\"\n    description: \"OAuth 2.1 for MCP clients, supports PKCE, token TTL 1h, refresh 30d.\"\n"
source_yaml_url: https://artifacts.apis.io/audiomap-ai/authentication/audiomap-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Transcription
- Audio
- Meeting Notes
- Europe
---
