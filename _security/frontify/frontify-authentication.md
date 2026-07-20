---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Frontify Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Frontify secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Frontify
provider_slug: frontify
scheme_count: 2
schemes:
- description: Interactive OAuth 2.0 authorization against a user's Frontify instance — used by the Frontify Authenticator, Finder, and the hosted MCP server (which follows the MCP authorization spec with CIMD and Dynamic Client Registration). Authorization/token endpoints are instance-scoped (https://{instance}.frontify.com).
  flow: authorizationCode
  name: OAuth2 (Authorization Code)
  sources:
  - developer.frontify.com
  - '@frontify/frontify-authenticator'
  - github.com/Frontify/mcp-servers
  type: oauth2
- description: Personal / API access tokens generated per Frontify instance are sent as a Bearer token when calling the GraphQL API directly (server-to-server).
  in: header
  name: API Token (Bearer)
  parameter: Authorization
  sources:
  - developer.frontify.com
  type: apiKey
slug: frontify-authentication
source_filename: frontify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://developer.frontify.com/ (GraphQL API + authentication docs) +\n  npm @frontify/frontify-authenticator + github.com/Frontify/mcp-servers\ndocs: https://developer.frontify.com/d/XFPcrX4jz6V8/graphql-api\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Derived from documentation and the official Frontify Authenticator package\n    rather than an OpenAPI spec (Frontify's public API is GraphQL; no OpenAPI is\n    published). Scope strings are intentionally not enumerated here — the exact\n    scope reference is behind the SPA developer portal and was not verified in\n    this pass, so no scopes/ artifact is asserted.\nschemes:\n  - name: OAuth2 (Authorization Code)\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      Interactive OAuth 2.0 authorization against a user's Frontify instance —\n      used by the Frontify Authenticator,\
  \ Finder, and the hosted MCP server\n      (which follows the MCP authorization spec with CIMD and Dynamic Client\n      Registration). Authorization/token endpoints are instance-scoped\n      (https://{instance}.frontify.com).\n    sources: [developer.frontify.com, \"@frontify/frontify-authenticator\", github.com/Frontify/mcp-servers]\n  - name: API Token (Bearer)\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      Personal / API access tokens generated per Frontify instance are sent as a\n      Bearer token when calling the GraphQL API directly (server-to-server).\n    sources: [developer.frontify.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontify/refs/heads/main/authentication/frontify-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Marketing
- Brand Management
- Digital Asset Management
- DAM
- Content
- GraphQL
- Creative Operations
---
