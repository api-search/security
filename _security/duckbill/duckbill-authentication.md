---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Duckbill Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Duckbill secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Duckbill
provider_slug: duckbill
scheme_count: 2
schemes:
- issuer: https://clerk.getduckbill.com
  name: OpenIDConnect
  openIdConnectUrl: https://clerk.getduckbill.com/.well-known/openid-configuration
  sources:
  - well-known/duckbill-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://clerk.getduckbill.com/oauth/authorize
    flow: authorizationCode
    introspectionUrl: https://clerk.getduckbill.com/oauth/token_info
    pkce_methods:
    - S256
    revocationUrl: https://clerk.getduckbill.com/oauth/token/revoke
    tokenUrl: https://clerk.getduckbill.com/oauth/token
    userinfoUrl: https://clerk.getduckbill.com/oauth/userinfo
  name: OAuth2
  sources:
  - well-known/duckbill-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: duckbill-authentication
source_filename: duckbill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://clerk.getduckbill.com/.well-known/openid-configuration\ndocs: https://getduckbill.com/platform\nnotes: >-\n  Duckbill has no public REST OpenAPI to derive from. Its programmatic surface\n  (the \"Connect to Claude\" MCP integration and platform/API access) authenticates\n  through an OAuth 2.0 / OpenID Connect authorization server hosted by Clerk on\n  Duckbill's own subdomain clerk.getduckbill.com. End-user app auth is also Clerk.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  identity_provider: Clerk (clerk.getduckbill.com)\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://clerk.getduckbill.com/.well-known/openid-configuration\n  issuer: https://clerk.getduckbill.com\n  sources: [well-known/duckbill-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.getduckbill.com/oauth/authorize\n\
  \    tokenUrl: https://clerk.getduckbill.com/oauth/token\n    revocationUrl: https://clerk.getduckbill.com/oauth/token/revoke\n    userinfoUrl: https://clerk.getduckbill.com/oauth/userinfo\n    introspectionUrl: https://clerk.getduckbill.com/oauth/token_info\n    pkce_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  sources: [well-known/duckbill-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duckbill/refs/heads/main/authentication/duckbill-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- AI Assistant
- Personal Assistant
- Task Automation
- Agents
- MCP
- Concierge
---
