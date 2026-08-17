---
api_key_in: []
auth_types:
- oauth2
- http-bearer
- saml2
description: 'DERIVED FROM DOCS, NOT FROM A SPEC — Grid publishes no OpenAPI, so there is no securitySchemes block to read. Everything below comes from Grid''s own help-center articles.

  Grid has two authentication stories and they are not the same surface. The AGENT surface (the remote MCP server) authenticates with OAuth 2.0, with a long-lived bearer access token offered only as a documented fallback for Claude Code. The HUMAN surface (the Grid web app) supports SAML 2.0 enterprise SSO against Okta and Microsoft Entra ID, configured by exchanging metadata with Grid support rather than self-serve in the app.

  There is no API key programme. No article in Grid''s knowledge base documents issuing, rotating, scoping or revoking an API credential for a REST API, because there is no public REST API.'
kind: authentication
layout: security
method: searched
name: Grid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grid secures its APIs with oauth2, http-bearer, and saml2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Grid
provider_slug: grid
scheme_count: 3
schemes:
- authorization_server: null
  authorization_server_note: Not published. /.well-known/oauth-authorization-server 404s on api.saasgrid.com and returns an SPA HTML shell (not metadata) on app.withgrid.com. See well-known/grid-well-known.yml.
  description: '"Use OAuth wherever it''s supported." The OAuth flow is completed inside the MCP client — /mcp in Claude Code, Connect in claude.ai settings, or the App authentication step in the ChatGPT admin console.'
  flow: authorization_code
  flow_note: Inferred from the interactive per-user consent flow the docs describe; Grid does not name the grant type and publishes no RFC 8414 authorization-server metadata, so the flow is not machine-confirmable.
  name: mcp-oauth
  oidc_note: Grid explicitly instructs ChatGPT admins to open Advanced OAuth settings and UNCHECK "OIDC enabled" — the authorization server is OAuth 2.0 only and does not present a working OIDC layer to that client.
  preferred: true
  scopes: []
  scopes_note: No scopes are published. The server is documented as read-only in the aggregate, but no per-scope or per-resource permission model is described.
  sources:
  - https://help.saasgrid.com/articles/5945378492-grid-mcp
  surface: MCP server (agent)
  type: oauth2
- description: 'Fallback for Claude Code only. The token is generated at https://app.withgrid.com/mcp-auth and passed as a static header: --header "Authorization: Bearer <Your token>".'
  expiry: null
  expiry_note: No lifetime, rotation policy, or revocation procedure is documented.
  format: Bearer <token>
  header: Authorization
  name: mcp-access-token
  preferred: false
  scheme: bearer
  sources:
  - https://help.saasgrid.com/articles/5945378492-grid-mcp
  surface: MCP server (agent)
  type: http
- description: SAML 2.0 single sign-on. Grid supplies a Single Sign-On URL and an Audience URI (SP Entity ID); the customer returns their IdP metadata URL to the Grid point of contact, who completes the connection.
  identity_platform: null
  identity_platform_note: Grid does not name an underlying identity vendor (WorkOS, Auth0, Okta Customer Identity) in its documentation.
  identity_providers:
  - exchange: Grid provides Single Sign-On URL + Audience URI (SP Entity ID); customer sends the Okta metadata URL to Grid.
    name: Okta
  - exchange: Grid provides the Reply URL (Assertion Consumer Service URL) + Identifier (Entity ID); customer sends the App Federation Metadata URL to Grid support.
    name: Microsoft Entra ID (Azure AD)
  name: enterprise-sso
  self_serve: false
  self_serve_note: Configuration is not available in-app; it requires a support-mediated metadata exchange with a named Grid point of contact.
  sources:
  - https://help.saasgrid.com/articles/9859006764-setting-up-sso-for-saasgrid
  surface: Grid web application (human)
  type: saml2
slug: grid-authentication
source_filename: grid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://help.saasgrid.com/articles/5945378492-grid-mcp +\n  https://help.saasgrid.com/articles/9859006764-setting-up-sso-for-saasgrid\ndocs:\n  - https://help.saasgrid.com/articles/5945378492-grid-mcp\n  - https://help.saasgrid.com/articles/9859006764-setting-up-sso-for-saasgrid\ndescription: >-\n  DERIVED FROM DOCS, NOT FROM A SPEC — Grid publishes no OpenAPI, so there is no\n  securitySchemes block to read. Everything below comes from Grid's own help-center articles.\n\n  Grid has two authentication stories and they are not the same surface. The AGENT surface\n  (the remote MCP server) authenticates with OAuth 2.0, with a long-lived bearer access token\n  offered only as a documented fallback for Claude Code. The HUMAN surface (the Grid web app)\n  supports SAML 2.0 enterprise SSO against Okta and Microsoft Entra ID, configured by\n  exchanging metadata with Grid support rather than self-serve in the app.\n\n  There\
  \ is no API key programme. No article in Grid's knowledge base documents issuing,\n  rotating, scoping or revoking an API credential for a REST API, because there is no public\n  REST API.\nsummary:\n  types:\n    - oauth2\n    - http-bearer\n    - saml2\n  api_key_programme: false\n  self_serve_credentials: partial\n  self_serve_note: >-\n    MCP OAuth and MCP access tokens are self-serve from https://app.withgrid.com/mcp-auth\n    once signed in, but enabling Grid as a connector in Claude or ChatGPT requires an org\n    admin, and SAML SSO requires a support-mediated metadata exchange.\nschemes:\n  - name: mcp-oauth\n    type: oauth2\n    surface: MCP server (agent)\n    preferred: true\n    description: >-\n      \"Use OAuth wherever it's supported.\" The OAuth flow is completed inside the MCP client\n      — /mcp in Claude Code, Connect in claude.ai settings, or the App authentication step in\n      the ChatGPT admin console.\n    flow: authorization_code\n    flow_note: >-\n     \
  \ Inferred from the interactive per-user consent flow the docs describe; Grid does not\n      name the grant type and publishes no RFC 8414 authorization-server metadata, so the\n      flow is not machine-confirmable.\n    authorization_server: null\n    authorization_server_note: >-\n      Not published. /.well-known/oauth-authorization-server 404s on api.saasgrid.com and\n      returns an SPA HTML shell (not metadata) on app.withgrid.com. See\n      well-known/grid-well-known.yml.\n    scopes: []\n    scopes_note: >-\n      No scopes are published. The server is documented as read-only in the aggregate, but\n      no per-scope or per-resource permission model is described.\n    oidc_note: >-\n      Grid explicitly instructs ChatGPT admins to open Advanced OAuth settings and UNCHECK\n      \"OIDC enabled\" — the authorization server is OAuth 2.0 only and does not present a\n      working OIDC layer to that client.\n    sources:\n      - https://help.saasgrid.com/articles/5945378492-grid-mcp\n\
  \  - name: mcp-access-token\n    type: http\n    scheme: bearer\n    surface: MCP server (agent)\n    preferred: false\n    description: >-\n      Fallback for Claude Code only. The token is generated at\n      https://app.withgrid.com/mcp-auth and passed as a static header:\n      --header \"Authorization: Bearer <Your token>\".\n    header: Authorization\n    format: Bearer <token>\n    expiry: null\n    expiry_note: No lifetime, rotation policy, or revocation procedure is documented.\n    sources:\n      - https://help.saasgrid.com/articles/5945378492-grid-mcp\n  - name: enterprise-sso\n    type: saml2\n    surface: Grid web application (human)\n    description: >-\n      SAML 2.0 single sign-on. Grid supplies a Single Sign-On URL and an Audience URI\n      (SP Entity ID); the customer returns their IdP metadata URL to the Grid point of\n      contact, who completes the connection.\n    identity_providers:\n      - name: Okta\n        exchange: >-\n          Grid provides Single Sign-On\
  \ URL + Audience URI (SP Entity ID); customer sends the\n          Okta metadata URL to Grid.\n      - name: Microsoft Entra ID (Azure AD)\n        exchange: >-\n          Grid provides the Reply URL (Assertion Consumer Service URL) + Identifier\n          (Entity ID); customer sends the App Federation Metadata URL to Grid support.\n    self_serve: false\n    self_serve_note: >-\n      Configuration is not available in-app; it requires a support-mediated metadata\n      exchange with a named Grid point of contact.\n    identity_platform: null\n    identity_platform_note: >-\n      Grid does not name an underlying identity vendor (WorkOS, Auth0, Okta Customer\n      Identity) in its documentation.\n    sources:\n      - https://help.saasgrid.com/articles/9859006764-setting-up-sso-for-saasgrid\nauthorization:\n  model: role-based\n  roles_doc: https://help.saasgrid.com/articles/7313064116-user-roles\n  note: >-\n    Grid documents user roles for the web application. No mapping between web-app\
  \ roles and\n    what the MCP server can read on a user's behalf is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grid/refs/heads/main/authentication/grid-authentication.yml
summary_line: oauth2/http-bearer/saml2 · 3 schemes
tags:
- Company
- Infrastructure
- Revenue Operations
- SaaS Metrics
- Billing
- Forecasting
- Financial Reporting
- FinOps
---
