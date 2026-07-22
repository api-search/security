---
api_key_in: []
auth_types:
- jwt
- oauth2
- basic
- custom
description: ''
kind: authentication
layout: security
method: searched
name: Unifyapps Authentication
name_suffix: Authentication
oauth_flows: []
overview: UnifyApps secures its APIs with jwt, oauth2, basic, and custom across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UnifyApps
provider_slug: unifyapps
scheme_count: 4
schemes:
- bearerFormat: JWT
  context: API Manager option for exposed APIs and MCP servers
  name: JWT
  scheme: bearer
  type: http
- context: API Manager option for delegated third-party authorization on exposed endpoints; embedded integrations use OAuth 2.0 identity providers (Client ID, Client Secret, Redirect URI) with session tokens passed to the Angular/Flutter SDKs.
  name: OAuth 2.0
  type: oauth2
- context: API Manager option for exposed endpoints
  name: Basic Auth
  scheme: basic
  type: http
- context: API Manager option for specialized security requirements
  name: Custom Authentication
  type: custom
slug: unifyapps-authentication
source_filename: unifyapps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://www.unifyapps.com/docs/unify-agentic-ai/configure-mcp-servers\nsource: https://www.unifyapps.com/docs\nsummary:\n  types: [jwt, oauth2, basic, custom]\n  context: >-\n    UnifyApps publishes no single public REST API; authentication applies to\n    the endpoints customers expose from the platform (workflows as APIs, MCP\n    servers) and to embedded integrations.\nschemes:\n  - name: JWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    context: API Manager option for exposed APIs and MCP servers\n  - name: OAuth 2.0\n    type: oauth2\n    context: >-\n      API Manager option for delegated third-party authorization on exposed\n      endpoints; embedded integrations use OAuth 2.0 identity providers\n      (Client ID, Client Secret, Redirect URI) with session tokens passed to\n      the Angular/Flutter SDKs.\n  - name: Basic Auth\n    type: http\n    scheme: basic\n    context: API Manager option for exposed\
  \ endpoints\n  - name: Custom Authentication\n    type: custom\n    context: API Manager option for specialized security requirements\nsso:\n  - >-\n    Platform sign-in supports enterprise SSO via OpenID identity providers\n    (e.g. Google OpenID SSO configuration documented in the Governance /\n    identity provider setup docs).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unifyapps/refs/heads/main/authentication/unifyapps-authentication.yml
summary_line: jwt/oauth2/basic/custom · 4 schemes
tags:
- Company
- Ai
- Agentic AI
- Integration Platform
- iPaaS
- Automation
- No Code
- Enterprise
- Data Replication
- MCP
---
