---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentage-io-openapi-generated.yml
  format: yaml
  label: agentage-io API
  slug: agentage-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentage-io/openapi/_ae-authored/agentage-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentage Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: agentage-io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: agentage-io
provider_slug: agentage-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.1 with PKCE, token issued by auth.agentage.io
  flows:
    authorizationCode:
      authorizationUrl: https://auth.agentage.io/authorize
      scopes:
        memory:read: Read memories
        memory:write: Write memories
      tokenUrl: https://auth.agentage.io/token
  type: oauth2
slug: agentage-io-authentication
source_filename: agentage-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://docs.agentage.io/rest-api.md\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 with PKCE, token issued by auth.agentage.io\n    bearerFormat: JWT\n    flows:\n      authorizationCode:\n        authorizationUrl: https://auth.agentage.io/authorize\n        tokenUrl: https://auth.agentage.io/token\n        scopes:\n          memory:read: Read memories\n          memory:write: Write memories\n"
source_yaml_url: https://artifacts.apis.io/agentage-io/authentication/agentage-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Memory
- Collaboration
- Privacy
- EU-Hosted
---
