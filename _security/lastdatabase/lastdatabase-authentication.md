---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lastdatabase-openapi.yml
  format: yaml
  label: LastDatabase Lead Search API
  slug: lead-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lastdatabase/refs/heads/main/openapi/lastdatabase-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lastdatabase Authentication
name_suffix: Authentication
oauth_flows: []
overview: LastDatabase secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LastDatabase
provider_slug: lastdatabase
scheme_count: 2
schemes:
- description: 'Active LastDatabase API key.


    Send the key in the Authorization header:


    Authorization: Bearer YOUR_API_KEY'
  key_management: API keys are generated from the customer API management area after choosing an API plan; customers can disable their own keys. Free allows 1 key, Pro up to 10, Enterprise up to 100.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lastdatabase-openapi.yml
  type: http
- authorizationUrl: https://lastdatabase.com/oauth/authorize
  flows:
  - authorization_code
  - refresh_token
  metadata: https://lastdatabase.com/.well-known/oauth-authorization-server
  name: mcpOAuth
  pkce: S256
  sources:
  - https://lastdatabase.com/.well-known/oauth-authorization-server
  - https://lastdatabase.com/docs/mcp
  surface: MCP server (https://lastdatabase.com/mcp)
  tokenUrl: https://lastdatabase.com/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: lastdatabase-authentication
source_filename: lastdatabase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: searched\nsource: openapi/lastdatabase-openapi.yml; https://lastdatabase.com/api; https://lastdatabase.com/docs/mcp\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Active LastDatabase API key.\n\n\n    Send the key in the Authorization header:\n\n\n    Authorization: Bearer YOUR_API_KEY'\n  sources:\n  - openapi/lastdatabase-openapi.yml\n  key_management: API keys are generated from the customer API management area after choosing an API plan; customers can disable their own keys.\n    Free allows 1 key, Pro up to 10, Enterprise up to 100.\n- name: mcpOAuth\n  type: oauth2\n  surface: MCP server (https://lastdatabase.com/mcp)\n  flows:\n  - authorization_code\n  - refresh_token\n  authorizationUrl: https://lastdatabase.com/oauth/authorize\n  tokenUrl: https://lastdatabase.com/oauth/token\n  pkce: S256\n  token_endpoint_auth_methods:\n  - none\n  metadata: https://lastdatabase.com/.well-known/oauth-authorization-server\n\
  \  sources:\n  - https://lastdatabase.com/.well-known/oauth-authorization-server\n  - https://lastdatabase.com/docs/mcp\ndocs: https://lastdatabase.com/docs/api/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lastdatabase/refs/heads/main/authentication/lastdatabase-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Contact Data
- Lead Generation
- B2B Data
- Email Verification
- Data Enrichment
- Sales Prospecting
- MCP
---
