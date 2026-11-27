---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Étincel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Étincel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Étincel
provider_slug: etincel-ai
scheme_count: 1
schemes:
- flows:
    clientCredentials:
      scopes:
        etincel:use: Use Etincel AI services
      tokenUrl: https://etincel.ai/api/mcp
  type: oauth2
slug: etincel-ai-authentication
source_filename: etincel-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: https://etincel.ai/.well-known/oauth-protected-resource\nschemes:\n  - type: oauth2\n    flows:\n      clientCredentials:\n        tokenUrl: https://etincel.ai/api/mcp\n        scopes:\n          etincel:use: \"Use Etincel AI services\"\n"
source_yaml_url: https://artifacts.apis.io/etincel-ai/authentication/etincel-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- MCP
- Writing
- Voice
- Claude
---
