---
api_key_in: []
auth_types: []
description: Authentication profile for every Instant surface an external client can reach. There is no OpenAPI to derive securitySchemes from — derive-authentication.py returned zero profiles — so this artifact is built from the provider's own documentation plus live unauthenticated probes of api.instant.so. Instant has no OAuth flow, no OIDC discovery and no published API-key header convention; the single documented programmatic credential is a project-scoped access token presented as an HTTP bearer token to the MCP endpoint.
kind: authentication
layout: security
method: searched
name: Instant Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instant Commerce declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Instant Commerce
provider_slug: instant-commerce
scheme_count: 3
schemes:
- checked: '2026-08-13'
  description: A long-lived access token created in the Instant dashboard under Settings → General → Access tokens. The full token is shown exactly once at creation and cannot be displayed again; the dashboard afterwards lists only a masked prefix, the creator, and the last-used timestamp.
  evidence:
  - body: '{"message":"Missing Authorization header","error":"Unauthorized","statusCode":401}'
    probe: POST https://api.instant.so/mcp (no Authorization header)
    status: 401
  - body: '{"message":"Invalid or revoked token","error":"Unauthorized","statusCode":401}'
    note: 'The distinct message proves the header name/scheme is `Authorization: Bearer <token>` and that revocation state is checked at request time.'
    probe: 'POST https://api.instant.so/mcp with Authorization: Bearer <invalid>'
    status: 401
  id: mcp-access-token
  issuance:
    naming: Each token is named for where it will be used (the docs use "Claude Desktop" as the example).
    one_time_display: true
    where: Instant dashboard → Settings → General → Access tokens → New token
    who_may_issue: Project owners and admins only.
  revocation:
    immediate: true
    note: Any client using a revoked token loses access immediately and revocation cannot be undone. Server-side enforcement confirmed by probe.
    reversible: false
    where: Settings → General → Access tokens → token menu → Revoke
  scheme: bearer
  scoping:
    granularity: project
    note: A token is scoped to the current project only, and is tied to the member who created it. If that member loses access to the project, their tokens for it are revoked automatically. The provider recommends one token per developer/client so individual tokens can be revoked in isolation.
    oauth_scopes: none
  status: beta
  surface: https://api.instant.so/mcp
  type: http
- description: The CLI authenticates through an interactive login triggered by any command requiring store access (`instant login`), with `instant whoami`, `instant refresh` (refresh the access token), `instant select` (switch organization/storefront) and `instant logout` managing session state. The token format, endpoint and lifetime are not published.
  docs: https://docs.instantcommerce.io/developer/getting-started/authentication
  id: cli-interactive-login
  surface: Instant CLI (@instantcommerce/cli)
  type: interactive
- description: The Instant Storefront SDK is an unauthenticated browser-side JavaScript API attached to the shopper's page by the Instant storefront script. It carries no credential and exposes no privileged operation — it toggles and refreshes the Instant cart UI and dispatches DOM events. Cart mutation is delegated to Shopify's own Ajax Cart API under the shopper's session.
  docs: https://docs.instant.so/en/articles/16068067-instant-storefront-sdk.md
  id: storefront-sdk-none
  surface: window.Instant.api (published storefront)
  type: none
slug: instant-commerce-authentication
source_filename: instant-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.instant.so/en/articles/16068062-access-tokens-and-mcp.md\ndescription: >-\n  Authentication profile for every Instant surface an external client can reach.\n  There is no OpenAPI to derive securitySchemes from — derive-authentication.py\n  returned zero profiles — so this artifact is built from the provider's own\n  documentation plus live unauthenticated probes of api.instant.so. Instant has\n  no OAuth flow, no OIDC discovery and no published API-key header convention;\n  the single documented programmatic credential is a project-scoped access token\n  presented as an HTTP bearer token to the MCP endpoint.\ndocs:\n  - https://docs.instant.so/en/articles/16068062-access-tokens-and-mcp.md\n  - https://docs.instantcommerce.io/developer/getting-started/authentication\nschemes:\n  - id: mcp-access-token\n    type: http\n    scheme: bearer\n    surface: https://api.instant.so/mcp\n    status: beta\n    description:\
  \ >-\n      A long-lived access token created in the Instant dashboard under\n      Settings → General → Access tokens. The full token is shown exactly once at\n      creation and cannot be displayed again; the dashboard afterwards lists only\n      a masked prefix, the creator, and the last-used timestamp.\n    issuance:\n      where: Instant dashboard → Settings → General → Access tokens → New token\n      who_may_issue: Project owners and admins only.\n      one_time_display: true\n      naming: >-\n        Each token is named for where it will be used (the docs use \"Claude\n        Desktop\" as the example).\n    scoping:\n      granularity: project\n      note: >-\n        A token is scoped to the current project only, and is tied to the member\n        who created it. If that member loses access to the project, their tokens\n        for it are revoked automatically. The provider recommends one token per\n        developer/client so individual tokens can be revoked in isolation.\n\
  \      oauth_scopes: none\n    revocation:\n      where: Settings → General → Access tokens → token menu → Revoke\n      immediate: true\n      reversible: false\n      note: >-\n        Any client using a revoked token loses access immediately and revocation\n        cannot be undone. Server-side enforcement confirmed by probe.\n    evidence:\n      - probe: POST https://api.instant.so/mcp (no Authorization header)\n        status: 401\n        body: '{\"message\":\"Missing Authorization header\",\"error\":\"Unauthorized\",\"statusCode\":401}'\n      - probe: 'POST https://api.instant.so/mcp with Authorization: Bearer <invalid>'\n        status: 401\n        body: '{\"message\":\"Invalid or revoked token\",\"error\":\"Unauthorized\",\"statusCode\":401}'\n        note: >-\n          The distinct message proves the header name/scheme is\n          `Authorization: Bearer <token>` and that revocation state is checked at\n          request time.\n    checked: '2026-08-13'\n  - id: cli-interactive-login\n\
  \    type: interactive\n    surface: Instant CLI (@instantcommerce/cli)\n    description: >-\n      The CLI authenticates through an interactive login triggered by any command\n      requiring store access (`instant login`), with `instant whoami`,\n      `instant refresh` (refresh the access token), `instant select` (switch\n      organization/storefront) and `instant logout` managing session state. The\n      token format, endpoint and lifetime are not published.\n    docs: https://docs.instantcommerce.io/developer/getting-started/authentication\n  - id: storefront-sdk-none\n    type: none\n    surface: window.Instant.api (published storefront)\n    description: >-\n      The Instant Storefront SDK is an unauthenticated browser-side JavaScript\n      API attached to the shopper's page by the Instant storefront script. It\n      carries no credential and exposes no privileged operation — it toggles and\n      refreshes the Instant cart UI and dispatches DOM events. Cart mutation is\n \
  \     delegated to Shopify's own Ajax Cart API under the shopper's session.\n    docs: https://docs.instant.so/en/articles/16068067-instant-storefront-sdk.md\nabsent:\n  - scheme: oauth2\n    note: >-\n      No OAuth flow is documented and no OAuth metadata is served —\n      /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource\n      and /.well-known/oauth-protected-resource/mcp all return 404 on\n      api.instant.so. MCP clients cannot perform dynamic client registration or\n      an authorization-code flow; the user must paste a dashboard-issued token.\n    checked: '2026-08-13'\n  - scheme: openIdConnect\n    note: /.well-known/openid-configuration returns 404 on every Instant host.\n    checked: '2026-08-13'\n  - scheme: mutualTLS\n    note: Not documented on any surface.\n    checked: '2026-08-13'\nend_user_auth:\n  note: >-\n    Human sign-in to the Instant dashboard is email magic-link or Google, with no\n    password, per the help center. This is end-user\
  \ authentication, not an API\n    credential, and is recorded for completeness only.\n  docs: https://docs.instant.so/en/articles/16068137-create-your-account-and-sign-in.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instant-commerce/refs/heads/main/authentication/instant-commerce-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Ai Enterprise Software
- E-Commerce
- Shopify
- No-Code
- Page Builder
- Artificial Intelligence
- AI Agents
- Conversion Rate Optimization
- Developer Tools
- MCP
- agent-native
---
