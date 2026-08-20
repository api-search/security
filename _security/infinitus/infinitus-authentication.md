---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- saml2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Infinitus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Infinitus secures its APIs with oauth2, openIdConnect, saml2, and http across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Infinitus
provider_slug: infinitus
scheme_count: 0
schemes: []
slug: infinitus-authentication
source_filename: infinitus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://support.infinitus.ai/ikb/ai-agent-security-guide.md\ndocs: https://support.infinitus.ai/ikb/ai-agent-security-guide.md\nnote: >-\n  Derived from no OpenAPI — Infinitus publishes no machine-readable spec. This\n  profile is SEARCHED from the provider's own public knowledge base (the AI Agent\n  Security Guide) plus the two RFC discovery documents served at\n  www.infinitus.ai/.well-known/. It describes two distinct authentication\n  surfaces that should not be conflated: (1) end-user sign-in to the Infinitus\n  customer portal, and (2) OAuth 2.0 for the MCP server on the WordPress\n  marketing host. The credential model for the backend REST/GraphQL API at\n  api.infinitusai.com is NOT publicly documented — see gaps below.\n\nsummary:\n  types: [oauth2, openIdConnect, saml2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  public_spec: false\n  surfaces: 2\n\nsurfaces:\n\n- surface: customer-portal\n  name:\
  \ Infinitus Customer Portal\n  url: https://customer.infinitusai.com\n  audience: end users (health systems, pharma, providers, payors)\n  source: https://support.infinitus.ai/ikb/ai-agent-security-guide.md\n  schemes:\n  - name: google-workspace-sso\n    type: oauth2\n    subtype: openIdConnect\n    provider: Google Workspace\n    quote: 'OAuth/SSO option to let users sign in with their corporate Google Workspace account'\n  - name: microsoft-entra-sso\n    type: oauth2\n    subtype: openIdConnect\n    provider: Microsoft Azure AD / Entra ID\n    quote: 'OAuth/SSO option to let users sign in with their corporate Microsoft Azure AD account'\n  - name: saml-sso\n    type: saml2\n    binding: SP-initiated only\n    quote: 'SSO option to sign in with SAML. Note: we currently only support SP (service provider) initiated flow'\n    limitation: IdP-initiated SAML is NOT supported.\n  - name: magic-link\n    type: passwordless\n    channel: email\n    note: Passwordless sign-in via emailed magic\
  \ link.\n  session:\n    token_type: JWT\n    token_name: ID token\n    token_lifetime_seconds: 3600\n    refresh_token: true\n    quote: 'ID token (JWT) which expires after 1 hour and a refresh token to automatically update the ID token'\n    inactivity_timeout_minutes: 15\n    inactivity_note: Automatic sign-out after 15 minutes of inactivity.\n  authorization:\n    model: RBAC\n    quote: 'RBAC (role based access control) system to manage permissions'\n    detail: Org admins assign roles that determine user access levels.\n\n- surface: mcp-server\n  name: Infinitus WordPress MCP server\n  url: https://www.infinitus.ai/wp-json/mcp/mcp-oauth-server\n  audience: MCP clients / agents\n  source: https://www.infinitus.ai/.well-known/oauth-authorization-server\n  schemes:\n  - name: oauth2-mcp\n    type: oauth2\n    flows:\n    - flow: authorizationCode\n      authorizationUrl: https://www.infinitus.ai/oauth/authorize\n      tokenUrl: https://www.infinitus.ai/oauth/token\n      revocationUrl:\
  \ https://www.infinitus.ai/oauth/revoke\n      pkce: S256\n      pkce_required: true\n      scopes:\n        mcp: Access the Model Context Protocol server\n    client_auth: none\n    client_auth_note: >-\n      token_endpoint_auth_methods_supported is [\"none\"] — public clients only,\n      protected by PKCE (S256) rather than a client secret.\n    client_id_metadata_document_supported: true\n    bearer_methods_supported: [header]\n    discovery:\n      authorization_server_metadata: https://www.infinitus.ai/.well-known/oauth-authorization-server\n      protected_resource_metadata: https://www.infinitus.ai/.well-known/oauth-protected-resource\n\nnetwork:\n  allowlist_required: true\n  quote: >-\n    whitelisting traffic to https://customer.infinitusai.com and\n    https://api.infinitusai.com on TCP port 443\n  hosts:\n  - https://customer.infinitusai.com\n  - https://api.infinitusai.com\n  port: 443\n  source: https://support.infinitus.ai/ikb/ai-agent-security-guide.md\n\ngaps:\n- gap:\
  \ backend-api-credentials-undocumented\n  detail: >-\n    Infinitus' own security guide names https://api.infinitusai.com as the\n    backend API host, but publishes no credential model for it. Probes show\n    GET /v1/tasks -> 401 and POST /graphql -> 401, both returning a bare\n    text/plain \"Unauthorized\" with NO WWW-Authenticate header, so the scheme\n    (bearer JWT vs API key vs mTLS) cannot be determined without a customer\n    account. Recorded as unknown rather than guessed.\n- gap: no-securityschemes\n  detail: No OpenAPI is published, so no securitySchemes could be derived.\n- gap: no-scope-reference\n  detail: >-\n    No scopes/permissions reference page exists for the product API. The only\n    published OAuth scope anywhere on the Infinitus surface is \"mcp\" — see\n    scopes/infinitus-scopes.yml.\n\nx-evidence:\n- fetched: '2026-08-15'\n  url: https://support.infinitus.ai/ikb/ai-agent-security-guide.md\n  http_status: 200\n  kind: provider-knowledge-base\n- fetched:\
  \ '2026-08-15'\n  url: https://www.infinitus.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  kind: rfc8414\n- fetched: '2026-08-15'\n  url: https://api.infinitusai.com/v1/tasks\n  http_status: 401\n  kind: negative-probe\n  detail: 'text/plain \"Unauthorized\", no WWW-Authenticate header'\n- fetched: '2026-08-15'\n  url: https://api.infinitusai.com/graphql\n  http_status: 401\n  kind: negative-probe\n  detail: 'introspection POST rejected: text/plain \"Unauthorized\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinitus/refs/heads/main/authentication/infinitus-authentication.yml
summary_line: oauth2/openIdConnect/saml2/http · 0 schemes
tags:
- Company
- Artificial Intelligence
- Healthcare
- Voice AI
- Benefit Verification
- Prior Authorization
- HIPAA
---
