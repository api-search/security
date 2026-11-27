---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eveoy-com-mcp-api-openapi.yml
  format: yaml
  label: Eveoy MCP API
  slug: eveoy-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eveoy-com/openapi/eveoy-com-mcp-api-openapi.yml
- filename: eveoy-com-order-api-openapi.yml
  format: yaml
  label: Eveoy Order API
  slug: eveoy-com-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eveoy-com/openapi/eveoy-com-order-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eveoy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Eveoy secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Eveoy
provider_slug: eveoy-com
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/token
  name: oauth2
  sources:
  - openapi/eveoy-com-openapi.json
  type: oauth2
slug: eveoy-com-authentication
source_filename: eveoy-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/eveoy-com-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/token\n    scopes: 3\n  sources:\n  - openapi/eveoy-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eveoy-com/authentication/eveoy-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CustomerPhotos
- InStoreSampling
- BuyAndTry
- Marketing
- Retail
---
