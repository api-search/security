---
anonymous_access: false
api_key_in: []
api_specs:
- filename: akkrudata-ai-openapi-generated.yml
  format: yaml
  label: AkkruData API
  slug: akkrudata-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/akkrudata-ai/openapi/_ae-authored/akkrudata-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AkkruData Authentication
name_suffix: Authentication
oauth_flows: []
overview: AkkruData declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AkkruData
provider_slug: akkrudata-ai
scheme_count: 1
schemes:
- authorizationUrl: https://api.akkrudata.ai/mcp/oauth/authorize
  description: OAuth sign‑in with AkkruData account (email/password, Google, GitHub)
  flow: authorization_code
  tokenUrl: https://api.akkrudata.ai/mcp/oauth/token
  type: oauth2
slug: akkrudata-ai-authentication
source_filename: akkrudata-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://www.akkrudata.ai/documents/mcp.md\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    description: OAuth sign‑in with AkkruData account (email/password, Google, GitHub)\n    tokenUrl: https://api.akkrudata.ai/mcp/oauth/token\n    authorizationUrl: https://api.akkrudata.ai/mcp/oauth/authorize\n"
source_yaml_url: https://artifacts.apis.io/akkrudata-ai/authentication/akkrudata-ai-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Data
- Artificial Intelligence
- Filings
---
