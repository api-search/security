---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CompSlate Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompSlate declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CompSlate
provider_slug: compslate-com
scheme_count: 2
schemes:
- applies_to: https://compslate.com/mcp
  bearer_methods:
  - header
  client_registration:
  - dynamic client registration (registration_endpoint https://compslate.com/register)
  - client ID metadata documents (client_id_metadata_document_supported true)
  description: Assistants such as Claude and ChatGPT connect with OAuth 2.1, and PKCE (S256) is required. You approve each connection yourself, signed in to your workspace.
  discovery:
  - http_status: 200
    url: https://compslate.com/.well-known/oauth-protected-resource
  - http_status: 200
    url: https://compslate.com/.well-known/oauth-authorization-server
  flows:
    authorizationCode:
      authorizationUrl: https://compslate.com/authorize
      refreshUrl: https://compslate.com/token
      scopes:
        comp: Access to the signed-in person's CompSlate workspace (scope named in the protected-resource document; no description published)
      tokenUrl: https://compslate.com/token
  identity: An assistant acts as the person who connected it and sees only what that person can see.
  name: oauth2
  pkce: S256 required
  revocation_endpoint: https://compslate.com/revoke
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  token_lifetimes:
    access_token: Access tokens last 1 hour.
    authorization_code: Authorization codes expire after 10 minutes and work once.
    refresh_token: 'Refresh tokens last 90 days and work only once: each use replaces them with a new pair.'
  type: oauth2
- applies_to: web app and the OAuth consent sign-in
  description: There are no passwords. You sign in with a one-time link emailed to you, which works once and expires after 20 minutes.
  name: email-magic-link
  session: Sessions last up to 30 days, in a cookie that scripts can't read (HttpOnly, SameSite=Lax, and Secure on our live site).
  type: passwordless-email-link
slug: compslate-com-authentication
source_filename: compslate-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://compslate.com/security\ndocs: https://compslate.com/docs/connect\nnote: CompSlate publishes no REST contract; the only programmatic surface is the remote MCP server at https://compslate.com/mcp. Values below are read from the docs, the security page and the provider's own OAuth discovery documents (fetched with GET).\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://compslate.com/mcp\n  description: 'Assistants such as Claude and ChatGPT connect with OAuth 2.1, and PKCE (S256) is required. You approve each connection yourself, signed in to your workspace.'\n  flows:\n    authorizationCode:\n      authorizationUrl: https://compslate.com/authorize\n      tokenUrl: https://compslate.com/token\n      refreshUrl: https://compslate.com/token\n      scopes:\n        comp: Access to the signed-in person's CompSlate workspace (scope named in the protected-resource document; no description published)\n  pkce: S256\
  \ required\n  client_registration:\n  - dynamic client registration (registration_endpoint https://compslate.com/register)\n  - client ID metadata documents (client_id_metadata_document_supported true)\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  revocation_endpoint: https://compslate.com/revoke\n  bearer_methods: [header]\n  token_lifetimes:\n    access_token: Access tokens last 1 hour.\n    refresh_token: 'Refresh tokens last 90 days and work only once: each use replaces them with a new pair.'\n    authorization_code: Authorization codes expire after 10 minutes and work once.\n  discovery:\n  - url: https://compslate.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://compslate.com/.well-known/oauth-authorization-server\n    http_status: 200\n  identity: An assistant acts as the person who connected it and sees only what that person can see.\n- name: email-magic-link\n  type: passwordless-email-link\n  applies_to: web\
  \ app and the OAuth consent sign-in\n  description: There are no passwords. You sign in with a one-time link emailed to you, which works once and expires after 20 minutes.\n  session: Sessions last up to 30 days, in a cookie that scripts can't read (HttpOnly, SameSite=Lax, and Secure on our live site).\n"
source_yaml_url: https://artifacts.apis.io/compslate-com/authentication/compslate-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Sales Compensation
- Sales Commissions
- Revenue Operations
- MCP
- AI Assistant
- Software-as-a-Service
---
