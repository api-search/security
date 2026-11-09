---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aiwatermarkremover Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Watermark Remover declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AI Watermark Remover
provider_slug: aiwatermarkremover-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: API key passed as Bearer token in Authorization header.
  scheme: bearer
  type: http
- description: OAuth flow for remote MCP server integration.
  flows:
    authorizationCode:
      authorizationUrl: https://aiwatermarkremover.com/auth/google
      scopes: {}
      tokenUrl: https://aiwatermarkremover.com/oauth/token
  type: oauth2
slug: aiwatermarkremover-com-authentication
source_filename: aiwatermarkremover-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://aiwatermarkremover.com/api-docs\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: API key passed as Bearer token in Authorization header.\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://aiwatermarkremover.com/auth/google\n        tokenUrl: https://aiwatermarkremover.com/oauth/token\n        scopes: {}\n    description: OAuth flow for remote MCP server integration.\n"
source_yaml_url: https://artifacts.apis.io/aiwatermarkremover-com/authentication/aiwatermarkremover-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Image Processing
- Watermark Removal
- Online Tool
- Free
---
