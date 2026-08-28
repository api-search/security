---
api_key_in:
- cookie
- header
api_specs:
- filename: medusa-store-openapi.yaml
  format: yaml
  label: Medusa Store API
  slug: medusa-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/openapi/medusa-store-openapi.yaml
- filename: medusa-admin-openapi.yaml
  format: yaml
  label: Medusa Admin API
  slug: medusa-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/openapi/medusa-admin-openapi.yaml
auth_types:
- http
- apiKey
description: 'Medusa authenticates with an actor type plus a method, not with a single key. The actor is `user` (admin), `customer`, or a custom actor type a merchant defines; the method is a JWT bearer token, a session cookie, or — for admin only — a secret API key. Route protection is by path prefix rather than by declared security on each operation, which is why neither published document sets a top-level `security` block: /admin is protected by default, /store/customers/me is protected for customers, and everything else under /store is public but still requires a publishable API key that scopes the request to a sales channel.'
kind: authentication
layout: security
method: searched
name: Medusa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medusa secures its APIs with http and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Medusa
provider_slug: medusa
scheme_count: 4
schemes:
- actors:
  - user
  - customer
  display_name: JWT Token
  header: 'Authorization: Bearer <token>'
  name: jwt_token
  obtained_via: POST /auth/{actor_type}/{auth_provider} (e.g. /auth/user/emailpass, /auth/customer/emailpass) returns a token. Third-party providers (Google, GitHub) are supported through auth provider modules.
  scheme: bearer
  sources:
  - openapi/medusa-admin-openapi.yaml
  - openapi/medusa-store-openapi.yaml
  type: http
- actors:
  - user
  - customer
  display_name: Cookie Session ID
  in: cookie
  name: cookie_auth
  obtained_via: POST /auth/session after obtaining a JWT; used by browser clients including the Medusa Admin.
  parameter: connect.sid
  sources:
  - openapi/medusa-admin-openapi.yaml
  - openapi/medusa-store-openapi.yaml
  type: apiKey
- actors:
  - user
  display_name: API Token
  name: api_token
  note: Admin only. This is the credential a server-to-server integration uses.
  obtained_via: A secret API key created in the Admin dashboard or via POST /admin/api-keys with type=secret. Sent as the HTTP Basic username with an empty password.
  scheme: basic
  sources:
  - openapi/medusa-admin-openapi.yaml
  type: http
- display_name: Reset Password Token
  name: reset_password
  note: A single-purpose token for the password-reset flow, flagged x-is-auth:false in the spec — it is not a general authentication scheme and should not be treated as one.
  scheme: bearer
  sources:
  - openapi/medusa-admin-openapi.yaml
  - openapi/medusa-store-openapi.yaml
  type: http
  x_is_auth: false
slug: medusa-authentication
source_filename: medusa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  Derived from components.securitySchemes in openapi/medusa-store-openapi.yaml and\n  openapi/medusa-admin-openapi.yaml (2.19.0) by 0-working/derive-authentication.py, then\n  upgraded from https://docs.medusajs.com/learn/fundamentals/api-routes/protected-routes,\n  https://docs.medusajs.com/api/store, https://docs.medusajs.com/api/admin and the probed\n  OAuth metadata in well-known/.\ndescription: >-\n  Medusa authenticates with an actor type plus a method, not with a single key. The actor is\n  `user` (admin), `customer`, or a custom actor type a merchant defines; the method is a JWT\n  bearer token, a session cookie, or — for admin only — a secret API key. Route protection\n  is by path prefix rather than by declared security on each operation, which is why neither\n  published document sets a top-level `security` block: /admin is protected by default,\n  /store/customers/me is protected for customers, and everything\
  \ else under /store is public\n  but still requires a publishable API key that scopes the request to a sales channel.\nsummary:\n  types: [http, apiKey]\n  schemes: 4\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  api_key_in: [cookie, header]\nschemes:\n  - name: jwt_token\n    type: http\n    scheme: bearer\n    display_name: JWT Token\n    actors: [user, customer]\n    sources: [openapi/medusa-admin-openapi.yaml, openapi/medusa-store-openapi.yaml]\n    obtained_via: >-\n      POST /auth/{actor_type}/{auth_provider} (e.g. /auth/user/emailpass,\n      /auth/customer/emailpass) returns a token. Third-party providers (Google, GitHub) are\n      supported through auth provider modules.\n    header: 'Authorization: Bearer <token>'\n  - name: cookie_auth\n    type: apiKey\n    in: cookie\n    parameter: connect.sid\n    display_name: Cookie Session ID\n    actors: [user, customer]\n    sources: [openapi/medusa-admin-openapi.yaml, openapi/medusa-store-openapi.yaml]\n    obtained_via:\
  \ POST /auth/session after obtaining a JWT; used by browser clients including the Medusa Admin.\n  - name: api_token\n    type: http\n    scheme: basic\n    display_name: API Token\n    actors: [user]\n    sources: [openapi/medusa-admin-openapi.yaml]\n    obtained_via: >-\n      A secret API key created in the Admin dashboard or via POST /admin/api-keys with\n      type=secret. Sent as the HTTP Basic username with an empty password.\n    note: Admin only. This is the credential a server-to-server integration uses.\n  - name: reset_password\n    type: http\n    scheme: bearer\n    display_name: Reset Password Token\n    x_is_auth: false\n    sources: [openapi/medusa-admin-openapi.yaml, openapi/medusa-store-openapi.yaml]\n    note: >-\n      A single-purpose token for the password-reset flow, flagged x-is-auth:false in the\n      spec — it is not a general authentication scheme and should not be treated as one.\nadditional_required_header:\n  name: x-publishable-api-key\n  applies_to: every\
  \ /store route\n  is_credential: false\n  purpose: >-\n    Scopes the request to one or more sales channels, so a storefront only sees the products\n    and inventory of its own channel. Created in the Admin dashboard, via POST\n    /admin/api-keys with type=publishable, or by createApiKeysWorkflow. Safe to ship in\n    client-side code.\n  docs: https://docs.medusajs.com/api/store#publishable-api-key\nroute_protection:\n  mechanism: path-prefix defaults plus an `authenticate` middleware\n  defaults:\n    - { prefix: /admin, access: authenticated admin users only }\n    - { prefix: /store/customers/me, access: authenticated customers only }\n    - { prefix: /store, access: public, but x-publishable-api-key is required }\n  opt_out: 'export const AUTHENTICATE = false in a route file disables the default requirement.'\n  custom: >-\n    authenticate(actorType, methods[, { allowUnauthenticated, allowUnregistered }]) applied\n    in src/api/middlewares.ts. Methods are session, bearer and —\
  \ for admin — api-key. A\n    merchant can define custom actor types (e.g. `manager`) with their own auth flow.\n  docs: https://docs.medusajs.com/learn/fundamentals/api-routes/protected-routes\nmfa:\n  supported: true\n  evidence: >-\n    Multi-Factor Authentication tags in both documents (Store: \"Multi-Factor Authentication\n    (MFA) Factors\"; Admin: \"Multi-Factor Authentication\"), plus auth.mfa_enabled,\n    auth.mfa_disabled and auth.mfa_recovery_codes_generated events in the published event\n    reference. Added in the 2.x line and announced in the June 2026 newsletter.\noauth:\n  rest_api: false\n  mcp_server: true\n  note: >-\n    OAuth appears nowhere in the REST contract. It exists only in front of the Medusa MCP\n    server, where authorization-code + PKCE (S256) with dynamic client registration is\n    advertised at https://docs.medusajs.com/.well-known/oauth-authorization-server. See\n    scopes/medusa-scopes.yml.\nscopes:\n  rest_api: none\n  note: >-\n    Neither key\
  \ type nor token carries scopes. Admin access is all-or-nothing for a `user`\n    actor; the only scoping mechanism in the product is the publishable key's sales-channel\n    binding on /store.\ngaps:\n  - No token expiry, refresh or rotation policy is documented for the JWT scheme.\n  - No per-key permission or scope model on Admin secret keys.\n  - No published key-prefix convention that would let a leaked credential be recognised by shape.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/authentication/medusa-authentication.yml
summary_line: http/apiKey · 4 schemes
tags:
- E-Commerce
- Headless Commerce
- Open-Source
- Commerce
- Storefront
- Order Management
- Node.js
- GraphQL
- Agentic Commerce
- MCP
---
