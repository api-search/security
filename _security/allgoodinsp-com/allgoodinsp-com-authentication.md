---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allgoodinsp-com-openapi-generated.yml
  format: yaml
  label: AllGoodInsp API
  slug: allgoodinsp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allgoodinsp-com/openapi/_ae-authored/allgoodinsp-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Allgoodinsp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AllGoodInsp declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AllGoodInsp
provider_slug: allgoodinsp-com
scheme_count: 2
schemes:
- description: API key passed as Bearer token in Authorization header.
  in: header
  name: Authorization
  type: apiKey
- authorizationUrl: https://allgoodinsp.com/login?redirect=%2Fdocs%2Fmcp
  description: Browser-based OAuth flow using Google sign‑in.
  flow: authorizationCode
  scopes: {}
  tokenUrl: https://allgoodinsp.com/oauth/token
  type: oauth2
slug: allgoodinsp-com-authentication
source_filename: allgoodinsp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://allgoodinsp.com/docs/mcp\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: API key passed as Bearer token in Authorization header.\n  - type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://allgoodinsp.com/login?redirect=%2Fdocs%2Fmcp\n    tokenUrl: https://allgoodinsp.com/oauth/token\n    scopes: {}\n    description: Browser-based OAuth flow using Google sign‑in.\n"
source_yaml_url: https://artifacts.apis.io/allgoodinsp-com/authentication/allgoodinsp-com-authentication.yml
summary_line: 2 schemes
tags:
- Design
- Artificial Intelligence
- References
- Curated
- MCP
---
