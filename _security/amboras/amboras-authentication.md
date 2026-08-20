---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Amboras Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amboras declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Amboras
provider_slug: amboras
scheme_count: 5
schemes:
- applies_to: Store API (/store/*)
  evidence: 'GET https://api.amboras.com/store/products with no header returns HTTP 400 {"type":"not_allowed","message":"Publishable API key required in the request header: x-publishable-api-key. You can manage your keys in settings in the dashboard."} (probed 2026-08-13). Amboras''s own storefront template documents the value as NEXT_PUBLIC_MEDUSA_PUBLISHABLE_KEY=pk_xxx, injected automatically by the dev orchestrator during store provisioning.'
  id: publishable-api-key
  in: header
  key_prefix: pk_
  name: x-publishable-api-key
  required: true
  type: apiKey
- applies_to: every call, Store and Admin
  evidence: '"The storefront sends X-Store-Environment-ID header on every Medusa API call via the JS SDK''s globalHeaders. The Medusa Backend Orchestrator routes queries to the correct store database." - Amboras storefront template README. This header is what makes the single api.amboras.com host multi-tenant; the CLAUDE.md notes the custom product-extensions endpoint "must include both headers".'
  id: store-environment-id
  in: header
  name: X-Store-Environment-ID
  required: true
  role: tenant selector, not a credential
  type: apiKey
- applies_to: Admin API (/admin/*)
  bearer_format: JWT
  evidence: GET https://api.amboras.com/admin returns HTTP 401 {"message":"Unauthorized"} (probed 2026-08-13). The /security page states "JWT-based authentication with refresh tokens" and "httpOnly cookies for secure token storage".
  id: admin-bearer
  scheme: bearer
  type: http
- applies_to: storefront customer accounts
  evidence: Amboras's published customer instructions name the exact calls - sdk.auth.login("customer", "emailpass", { email, password }) and sdk.auth.register("customer", "emailpass", { email, password }) - and state "Customer auth uses Medusa's built-in auth system, not Supabase" and "Session tokens are handled via the Medusa JS SDK automatically".
  id: customer-emailpass
  type: password
- applies_to: Amboras admin dashboard sign-in
  evidence: '"OAuth integration (Google, GitHub)" listed under Authentication and access control on https://www.amboras.com/security. No authorization-server metadata is published - /.well-known/openid-configuration and /.well-known/oauth-authorization-server return 404 on www., api. and admin.amboras.com - and no scope reference is documented, so no scopes/ artifact is emitted.'
  id: oauth-social
  providers:
  - Google
  - GitHub
  type: oauth2
slug: amboras-authentication
source_filename: amboras-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://github.com/Amboras/store-my-store-ju0t/blob/main/storefront/CLAUDE.md\ndocs:\n  - https://www.amboras.com/security\n  - https://github.com/Amboras/store-my-store-ju0t/blob/main/README.md\n  - https://github.com/Amboras/store-my-store-ju0t/blob/main/storefront/CLAUDE.md\nnote: >-\n  Amboras publishes no OpenAPI, so this profile is not derived from securitySchemes. It is\n  read from two provider-published sources - the /security page on amboras.com and the\n  storefront template Amboras ships in its own public GitHub organization - and confirmed\n  against live unauthenticated probes of https://api.amboras.com on 2026-08-13. The backend\n  is a multi-tenant Medusa v2 deployment Amboras operates; the auth mechanisms below are the\n  ones Amboras's own documentation instructs its storefronts to use.\nbase_url: https://api.amboras.com\nschemes:\n  - id: publishable-api-key\n    type: apiKey\n    in: header\n    name: x-publishable-api-key\n\
  \    applies_to: Store API (/store/*)\n    key_prefix: pk_\n    required: true\n    evidence: >-\n      GET https://api.amboras.com/store/products with no header returns HTTP 400\n      {\"type\":\"not_allowed\",\"message\":\"Publishable API key required in the request header:\n      x-publishable-api-key. You can manage your keys in settings in the dashboard.\"}\n      (probed 2026-08-13). Amboras's own storefront template documents the value as\n      NEXT_PUBLIC_MEDUSA_PUBLISHABLE_KEY=pk_xxx, injected automatically by the dev\n      orchestrator during store provisioning.\n  - id: store-environment-id\n    type: apiKey\n    in: header\n    name: X-Store-Environment-ID\n    applies_to: every call, Store and Admin\n    required: true\n    role: tenant selector, not a credential\n    evidence: >-\n      \"The storefront sends X-Store-Environment-ID header on every Medusa API call via the\n      JS SDK's globalHeaders. The Medusa Backend Orchestrator routes queries to the correct\n    \
  \  store database.\" - Amboras storefront template README. This header is what makes the\n      single api.amboras.com host multi-tenant; the CLAUDE.md notes the custom\n      product-extensions endpoint \"must include both headers\".\n  - id: admin-bearer\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    applies_to: Admin API (/admin/*)\n    evidence: >-\n      GET https://api.amboras.com/admin returns HTTP 401 {\"message\":\"Unauthorized\"}\n      (probed 2026-08-13). The /security page states \"JWT-based authentication with refresh\n      tokens\" and \"httpOnly cookies for secure token storage\".\n  - id: customer-emailpass\n    type: password\n    applies_to: storefront customer accounts\n    evidence: >-\n      Amboras's published customer instructions name the exact calls -\n      sdk.auth.login(\"customer\", \"emailpass\", { email, password }) and\n      sdk.auth.register(\"customer\", \"emailpass\", { email, password }) - and state\n      \"Customer auth uses Medusa's\
  \ built-in auth system, not Supabase\" and \"Session tokens\n      are handled via the Medusa JS SDK automatically\".\n  - id: oauth-social\n    type: oauth2\n    applies_to: Amboras admin dashboard sign-in\n    providers:\n      - Google\n      - GitHub\n    evidence: >-\n      \"OAuth integration (Google, GitHub)\" listed under Authentication and access control on\n      https://www.amboras.com/security. No authorization-server metadata is published -\n      /.well-known/openid-configuration and /.well-known/oauth-authorization-server return\n      404 on www., api. and admin.amboras.com - and no scope reference is documented, so no\n      scopes/ artifact is emitted.\naccess_control:\n  rbac: true\n  roles:\n    - Admin\n    - Member\n  scope: per-store permissions\n  mfa: available\n  evidence: >-\n    \"Role-based access control (RBAC)\" and \"Multi-factor authentication (MFA) available\" on\n    /security; the 2026-05-28 changelog entry \"Invite your team\" documents \"Admin or Member\n\
  \    roles and per-store permissions. Email invites, token-based onboarding\".\n  scim: enterprise-tier only\ngaps:\n  - No published API reference, developer portal or OpenAPI describing these schemes; the\n    only machine-adjacent documentation is the storefront template Amboras publishes on GitHub.\n  - No OAuth scope reference and no authorization-server metadata document.\n  - Publishable keys are described as managed \"in settings in the dashboard\" (admin.amboras.com),\n    which is behind a merchant login - key issuance is not self-service documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amboras/refs/heads/main/authentication/amboras-authentication.yml
summary_line: 5 schemes
tags:
- Company
- E-Commerce
- Artificial Intelligence
- Generative AI
- Automation
- Conversion Rate Optimization
- Retail
- No-Code Store Builder
- Y Combinator
- Agentic Commerce
- Storefront
- Payments
- Checkout
- Analytics
- Headless Commerce
- Medusa
- Plugins
- Multi-Tenant
---
