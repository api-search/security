---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Segmentstream Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SegmentStream secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SegmentStream
provider_slug: segmentstream
scheme_count: 1
schemes:
- bearer_methods:
  - header
  description: SegmentStream's MCP server is a public OAuth 2.0 client using the authorization-code flow with PKCE (S256) and RFC 7591 dynamic client registration. Sign-in happens in the browser and grants the agent the same permissions as the signed-in SegmentStream user (read-only reporting by default). Discoverable via RFC 8414 / RFC 9728 metadata.
  flows:
  - authorizationUrl: https://mcp.segmentstream.com/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://mcp.segmentstream.com/oauth/register
    tokenUrl: https://mcp.segmentstream.com/oauth/token
  name: OAuth2
  resource: https://mcp.segmentstream.com/mcp
  sources:
  - well-known/segmentstream-oauth-authorization-server.json
  - well-known/segmentstream-oauth-protected-resource.json
  type: oauth2
slug: segmentstream-authentication
source_filename: segmentstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://mcp.segmentstream.com/.well-known/oauth-authorization-server +\n  https://docs.segmentstream.com/mcp/getting-started\ndocs: https://docs.segmentstream.com/mcp/getting-started\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [none]     # public client (PKCE)\nschemes:\n  - name: OAuth2\n    type: oauth2\n    description: >-\n      SegmentStream's MCP server is a public OAuth 2.0 client using the\n      authorization-code flow with PKCE (S256) and RFC 7591 dynamic client\n      registration. Sign-in happens in the browser and grants the agent the\n      same permissions as the signed-in SegmentStream user (read-only reporting\n      by default). Discoverable via RFC 8414 / RFC 9728 metadata.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.segmentstream.com/oauth/authorize\n  \
  \      tokenUrl: https://mcp.segmentstream.com/oauth/token\n        registrationUrl: https://mcp.segmentstream.com/oauth/register\n    bearer_methods: [header]\n    resource: https://mcp.segmentstream.com/mcp\n    sources:\n      - well-known/segmentstream-oauth-authorization-server.json\n      - well-known/segmentstream-oauth-protected-resource.json\nnotes: >-\n  No public REST OpenAPI is published (docs reference an openapi.json that\n  currently 404s), so this profile is derived from the OAuth discovery metadata\n  the MCP server publishes rather than from an OpenAPI securitySchemes block.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segmentstream/refs/heads/main/authentication/segmentstream-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Marketing Analytics
- Attribution
- Marketing Measurement
- Advertising
- Budget Optimization
- Incrementality
- BigQuery
- MCP
- AI Agents
---
