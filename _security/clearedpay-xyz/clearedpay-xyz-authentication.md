---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clearedpay-xyz-v1-openapi.json
  format: json
  label: Cleared Protocol API V1 API
  slug: cleared-protocol-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearedpay-xyz/openapi/_original/clearedpay-xyz-v1-openapi.json
auth_types: []
description: Authentication methods for Cleared API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Clearedpay Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cleared declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cleared
provider_slug: clearedpay-xyz
scheme_count: 3
schemes:
- evidence: 'Send all four headers on every authenticated request, including GET: Header Value x-cleared-key Full clr_pk_... key ID x-cleared-ts 13-digit Unix-millisecond timestamp x-cleared-nonce Fresh unique nonce, for example a UUID Authorization CLEARED-HMAC followed by a standard base64 signature'
  header: x-cleared-key, x-cleared-ts, x-cleared-nonce, Authorization
  how_to_obtain: Create an API key in the dashboard, which provides a public clr_pk_ key ID and a clr_sk_ secret. The secret is used to compute the HMAC signature.
  location: header
  name: HMAC
  type: other
- authorize_url: https://api.clearedpay.xyz/mcp
  evidence: Cleared supports authorization code with S256 PKCE and dynamic client registration. Sign in through the browser, select an organization and network, and explicitly approve permissions.
  header: Authorization
  how_to_obtain: Use the hosted MCP client to perform the OAuth authorization code flow with PKCE; the client receives an opaque access token beginning clr_oat_.
  location: header
  name: Hosted MCP OAuth
  scopes:
  - invoice:read
  - customer:read
  - dashboard:read
  - invoice:write
  - customer:write
  type: oauth2
- evidence: 'Use Authorization: Bearer <Privy access token> for user routes. Obtain the token through the signed-in Privy session; Cleared API-key secrets cannot be substituted.'
  header: Authorization
  how_to_obtain: Sign in to the Cleared web UI; the Privy session provides a JWT access token.
  location: header
  name: Privy JWT
  type: http-bearer
slug: clearedpay-xyz-authentication
source_filename: clearedpay-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://clearedpay.xyz/docs/guides/api-keys
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://clearedpay.xyz/docs/guides/api-keys\nsources:\n- https://clearedpay.xyz/docs/guides/api-keys\n- https://clearedpay.xyz/docs/api/authentication\n- https://clearedpay.xyz/docs/mcp/overview\n- https://clearedpay.xyz/docs/guides/share-invoices\ndescription: Authentication methods for Cleared API\nschemes:\n- type: other\n  name: HMAC\n  evidence: 'Send all four headers on every authenticated request, including GET: Header Value x-cleared-key Full clr_pk_... key ID x-cleared-ts\n    13-digit Unix-millisecond timestamp x-cleared-nonce Fresh unique nonce, for example a UUID Authorization CLEARED-HMAC followed by a standard\n    base64 signature'\n  location: header\n  header: x-cleared-key, x-cleared-ts, x-cleared-nonce, Authorization\n  how_to_obtain: Create an API key in the dashboard, which provides a public clr_pk_ key ID and a clr_sk_ secret. The secret is used to compute\n\
  \    the HMAC signature.\n- type: oauth2\n  name: Hosted MCP OAuth\n  evidence: Cleared supports authorization code with S256 PKCE and dynamic client registration. Sign in through the browser, select an organization\n    and network, and explicitly approve permissions.\n  location: header\n  header: Authorization\n  authorize_url: https://api.clearedpay.xyz/mcp\n  scopes:\n  - invoice:read\n  - customer:read\n  - dashboard:read\n  - invoice:write\n  - customer:write\n  how_to_obtain: Use the hosted MCP client to perform the OAuth authorization code flow with PKCE; the client receives an opaque access token\n    beginning clr_oat_.\n- type: http-bearer\n  name: Privy JWT\n  evidence: 'Use Authorization: Bearer <Privy access token> for user routes. Obtain the token through the signed-in Privy session; Cleared API-key\n    secrets cannot be substituted.'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in to the Cleared web UI; the Privy session provides a JWT access token.\n\
  docs: https://clearedpay.xyz/docs/guides/api-keys\n"
source_yaml_url: https://artifacts.apis.io/clearedpay-xyz/authentication/clearedpay-xyz-authentication.yml
summary_line: 3 schemes
tags:
- Payments
- USDC
- Invoicing
- Blockchain
- Contractor
---
