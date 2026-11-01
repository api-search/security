---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Royalty Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: royalty-technology declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: royalty-technology
provider_slug: royalty-technology
scheme_count: 1
schemes:
- authorizationUrl: https://api.royalty.technology/oauth/authorize
  description: RoyalTea acts as its own OAuth 2.1 authorization server with PKCE (S256), Dynamic Client Registration (RFC 7591), and resource indicators (RFC 8707).
  flow: authorization_code
  pkce: true
  registrationUrl: https://api.royalty.technology/oauth/register
  tokenUrl: https://api.royalty.technology/oauth/token
  type: oauth2
slug: royalty-technology-authentication
source_filename: royalty-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://royalty.technology/docs/mcp\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    pkce: true\n    description: \"RoyalTea acts as its own OAuth 2.1 authorization server with PKCE (S256), Dynamic Client Registration (RFC 7591), and resource indicators (RFC 8707).\"\n    tokenUrl: https://api.royalty.technology/oauth/token\n    authorizationUrl: https://api.royalty.technology/oauth/authorize\n    registrationUrl: https://api.royalty.technology/oauth/register\n"
source_yaml_url: https://artifacts.apis.io/royalty-technology/authentication/royalty-technology-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Game Development
- Collaboration
- Revenue Sharing
- SaaS
---
