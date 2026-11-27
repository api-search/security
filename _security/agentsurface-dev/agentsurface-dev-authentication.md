---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentsurface-dev-docs-api-openapi.yml
  format: yaml
  label: Agent Surface Docs API
  slug: agentsurface-dev-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsurface-dev/openapi/agentsurface-dev-docs-api-openapi.yml
- filename: agentsurface-dev-md-api-openapi.yml
  format: yaml
  label: Agent Surface Md API
  slug: agentsurface-dev-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsurface-dev/openapi/agentsurface-dev-md-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agent Surface Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Surface declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Surface
provider_slug: agentsurface-dev
scheme_count: 3
schemes:
- description: Simple API key authentication for agents.
  in: header
  name: X-API-Key
  type: apiKey
- description: OAuth2 client credentials flow for agents.
  flows:
    clientCredentials:
      scopes:
        read: Read access
        write: Write access
      tokenUrl: https://agentsurface.dev/oauth/token
  type: oauth2
- description: DPoP proof-of-possession tokens for enhanced security.
  type: dpop
slug: agentsurface-dev-authentication
source_filename: agentsurface-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://agentsurface.dev/docs/authentication.md\nschemes:\n  - type: apiKey\n    name: \"X-API-Key\"\n    in: header\n    description: \"Simple API key authentication for agents.\"\n  - type: oauth2\n    flows:\n      clientCredentials:\n        tokenUrl: \"https://agentsurface.dev/oauth/token\"\n        scopes:\n          read: \"Read access\"\n          write: \"Write access\"\n    description: \"OAuth2 client credentials flow for agents.\"\n  - type: dpop\n    description: \"DPoP proof-of-possession tokens for enhanced security.\"\n"
source_yaml_url: https://artifacts.apis.io/agentsurface-dev/authentication/agentsurface-dev-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Agents
- Documentation
- Integration
---
