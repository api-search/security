---
api_key_in:
- header
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Driver Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Driver secures its APIs with oauth2, http, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Driver
provider_slug: driver
scheme_count: 4
schemes:
- authorizationUrl: https://api.us1.driverai.com/mcp/authorize
  flow: authorizationCode
  name: oauth2
  pkce: S256
  registrationUrl: https://api.us1.driverai.com/mcp/register
  revocationUrl: https://api.us1.driverai.com/mcp/revoke
  scopes:
  - openid
  - profile
  - email
  source: https://api.us1.driverai.com/.well-known/oauth-authorization-server
  tokenUrl: https://api.us1.driverai.com/mcp/token
  type: oauth2
- description: Personal access tokens authenticate as the user and inherit the user's organization role and source access. Expire in 30/90/180/365 days.
  header: Authorization
  in: header
  name: personal_access_token
  scheme: bearer
  token_prefix: drvp_
  type: http
- description: Machine identities for headless/M2M access. Bearer scheme; prefix routes to API-key auth automatically (no OAuth flow). Role-based per-source grants (Source Admin / Source Member), directly or via teams; no org-wide access.
  header: Authorization
  in: header
  name: machine_api_key
  scheme: bearer
  token_prefix: drvm_
  type: apiKey
- description: Enterprise SSO via SAML 2.0 (Okta, Microsoft Entra, Google Workspace, etc.), with SCIM 2.0 automated user provisioning. Requires Org Admin to configure.
  name: sso_saml
  type: saml2
slug: driver-authentication
source_filename: driver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.driver.ai/docs/personal-access-tokens\ndocs: https://www.driver.ai/docs/mcp-setup\nsummary:\n  types: [oauth2, http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Driver authenticates API and MCP requests three ways: OAuth 2.1 (browser\n    login, RFC 8414 authorization-server metadata published), Personal Access\n    Tokens (drvp_ prefix, authenticate as the user), and Machine API keys\n    (drvm_ prefix, machine-to-machine). Enterprise SSO uses SAML 2.0 with SCIM\n    provisioning.\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  authorizationUrl: https://api.us1.driverai.com/mcp/authorize\n  tokenUrl: https://api.us1.driverai.com/mcp/token\n  revocationUrl: https://api.us1.driverai.com/mcp/revoke\n  registrationUrl: https://api.us1.driverai.com/mcp/register   # RFC 7591 dynamic client registration\n  scopes: [openid, profile, email]\n\
  \  source: https://api.us1.driverai.com/.well-known/oauth-authorization-server\n- name: personal_access_token\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  token_prefix: drvp_\n  description: >-\n    Personal access tokens authenticate as the user and inherit the user's\n    organization role and source access. Expire in 30/90/180/365 days.\n- name: machine_api_key\n  type: apiKey\n  in: header\n  header: Authorization\n  scheme: bearer\n  token_prefix: drvm_\n  description: >-\n    Machine identities for headless/M2M access. Bearer scheme; prefix routes to\n    API-key auth automatically (no OAuth flow). Role-based per-source grants\n    (Source Admin / Source Member), directly or via teams; no org-wide access.\n- name: sso_saml\n  type: saml2\n  description: >-\n    Enterprise SSO via SAML 2.0 (Okta, Microsoft Entra, Google Workspace, etc.),\n    with SCIM 2.0 automated user provisioning. Requires Org Admin to configure.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/driver/refs/heads/main/authentication/driver-authentication.yml
summary_line: oauth2/http/apiKey · 4 schemes
tags:
- Company
- AI
- Developer Tools
- Code Documentation
- MCP
- Codebase Intelligence
- Agents
- Developer Experience
---
