---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: A2A Cosmetics Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: A2A Cosmetics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: A2A Cosmetics
provider_slug: a2a-cosmetics-ai
scheme_count: 1
schemes:
- authorizationUrl: null
  description: OAuth2 client credentials flow for accessing transacting tools on the MCP door. Tokens are JWTs signed with ES256 (kid a2ac-as-2026-09).
  flow: client_credentials
  revocationUrl: https://a2a-registry.ai/oauth/revoke
  scopes:
  - cosmetics.read
  - cosmetics.transact
  tokenUrl: https://a2a-registry.ai/oauth/token
  type: oauth2
slug: a2a-cosmetics-ai-authentication
source_filename: a2a-cosmetics-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://a2a-cosmetics.ai/auth.md\nschemes:\n  - type: oauth2\n    flow: client_credentials\n    tokenUrl: https://a2a-registry.ai/oauth/token\n    authorizationUrl: null\n    revocationUrl: https://a2a-registry.ai/oauth/revoke\n    scopes:\n      - cosmetics.read\n      - cosmetics.transact\n    description: \"OAuth2 client credentials flow for accessing transacting tools on the MCP door. Tokens are JWTs signed with ES256 (kid a2ac-as-2026-09).\"\n"
source_yaml_url: https://artifacts.apis.io/a2a-cosmetics-ai/authentication/a2a-cosmetics-ai-authentication.yml
summary_line: 1 scheme
tags:
- Cosmetics
- Artificial Intelligence
- AI Agents
- Commerce
- GTIN
---
