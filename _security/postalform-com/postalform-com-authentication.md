---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: postalform-com-machine-payments-openapi.json
  format: json
  label: PostalForm Machine Payments API
  slug: postalform-machine-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postalform-com/refs/heads/main/openapi/postalform-com-machine-payments-openapi.json
- filename: postalform-com-projects-openapi.json
  format: json
  label: PostalForm Projects Public API
  slug: postalform-projects-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postalform-com/refs/heads/main/openapi/postalform-com-projects-openapi.json
auth_types:
- http
- none
- payment-gated
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Postalform Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: PostalForm secures its APIs with http, none, and payment-gated across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PostalForm
provider_slug: postalform-com
scheme_count: 3
schemes:
- applied_to: 'all 25 operations (per-operation security [{bearerAuth: []}]; no global security block)'
  credential: workspace API key
  header_example: 'Authorization: Bearer pf_test_...'
  issuance: https://projects.postalform.com/signup (dashboard) or Stripe Projects provisioning of postalform/mail, which returns POSTALFORM_TEST_API_KEY and POSTALFORM_LIVE_API_KEY
  key_prefixes:
    live: pf_live_
    test: pf_test_
  name: bearerAuth
  rotation: 'POST /api/v1/api-keys/rotate {mode: test|live} -> ApiKeyRotation {api_key (returned once), api_key_prefix}; GET /api/v1/api-keys lists prefixes and status active|disabled|revoked with last_used_at'
  scheme: bearer
  scopes: none (one key per mode; no scoped permissions documented)
  sources:
  - openapi/postalform-com-projects-openapi.json
  - https://postalform.com/developer-mail-api
  surface: PostalForm Projects Public API (https://projects.postalform.com/api/v1)
  type: http
- applied_to: all 17 operations
  gate: 'HTTP 402. x402 family: PAYMENT-REQUIRED challenge, PAYMENT-SIGNATURE on retry, PAYMENT-RESPONSE on success (USDC on Base). MPP family: one WWW-Authenticate: Payment challenge per method (tempo, stripe, card), Authorization: Payment on retry, Payment-Receipt on success. Reads (forms catalog, schemas, order status) and validate endpoints are open.'
  name: none (payment-gated)
  note: 'The OpenAPI declares "security": [] at the top level and no components.securitySchemes — an accurate declaration of "no authentication", not an omission.'
  sources:
  - openapi/postalform-com-machine-payments-openapi.json
  - https://postalform.com/agents
  surface: PostalForm Machine Payments API (https://postalform.com/api/machine/*)
  type: none
- applied_to: initialize, tools/list, resources/list, read-only tools
  gate_on_writes: hosted checkout_url (human pays on Stripe-hosted page); complete_checkout with a Stripe shared payment token (spt_..., provider stripe); postalform.create_machine_order 402 challenge retried with payment_authorization (MPP) or payment_signature (x402). UCP calls additionally require a platform profile in _meta.ucp.profile.
  name: none (MCP)
  rfc9728: not served — /.well-known/oauth-protected-resource 404 on the MCP host
  sources:
  - https://postalform.com/.well-known/mcp.json
  - https://postalform.com/developers
  - https://postalform.com/.well-known/capability-card.json
  surface: MCP server (https://postalform.com/mcp) and its UCP (/ucp/mcp) and ACP (/acp/mcp) siblings
  type: none
slug: postalform-com-authentication
source_filename: postalform-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://postalform.com/developers\nderived_from:\n- openapi/postalform-com-projects-openapi.json\n- openapi/postalform-com-machine-payments-openapi.json\ndocs:\n- https://postalform.com/developer-mail-api\n- https://postalform.com/agents\n- https://postalform.com/.well-known/mcp.json\nsummary:\n  types: [http, none, payment-gated]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Only ONE of PostalForm's three surfaces uses a credential. The Projects API declares a single http bearer\n    scheme (bearerAuth) applied per operation to all 25 operations; the bearer is a workspace API key with a\n    documented prefix — pf_test_ for the free simulated environment, pf_live_ for real mail on prepaid\n    credits — rotated by POST /api/v1/api-keys/rotate {mode}, which returns the secret once. The Machine\n    Payments API declares NO securitySchemes and an empty top-level security[]; every paid operation is\n    gated by\
  \ an HTTP 402 payment challenge (x402 PAYMENT-REQUIRED / MPP WWW-Authenticate: Payment) rather\n    than by identity, and the free reads and validates need nothing. The MCP server requires no credential\n    to connect, initialize or list tools (\"No API key is required for the hosted MCP endpoint today\";\n    \"contact support@postalform.com for allowlisting\"), and its money-moving tools are gated by hosted\n    checkout, a buyer-approved Stripe shared payment token or the same 402 challenges. No OAuth 2.0 or OIDC\n    exists on any host (/.well-known/oauth-authorization-server, oauth-protected-resource and\n    openid-configuration all 404 on postalform.com and projects.postalform.com).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: PostalForm Projects Public API (https://projects.postalform.com/api/v1)\n  applied_to: 'all 25 operations (per-operation security [{bearerAuth: []}]; no global security block)'\n  credential: workspace API key\n  key_prefixes:\
  \ {test: pf_test_, live: pf_live_}\n  header_example: 'Authorization: Bearer pf_test_...'\n  issuance: 'https://projects.postalform.com/signup (dashboard) or Stripe Projects provisioning of postalform/mail, which returns POSTALFORM_TEST_API_KEY and POSTALFORM_LIVE_API_KEY'\n  rotation: 'POST /api/v1/api-keys/rotate {mode: test|live} -> ApiKeyRotation {api_key (returned once), api_key_prefix}; GET /api/v1/api-keys lists prefixes and status active|disabled|revoked with last_used_at'\n  scopes: none (one key per mode; no scoped permissions documented)\n  sources: [openapi/postalform-com-projects-openapi.json, https://postalform.com/developer-mail-api]\n- name: none (payment-gated)\n  type: none\n  surface: PostalForm Machine Payments API (https://postalform.com/api/machine/*)\n  applied_to: all 17 operations\n  gate: >-\n    HTTP 402. x402 family: PAYMENT-REQUIRED challenge, PAYMENT-SIGNATURE on retry, PAYMENT-RESPONSE on\n    success (USDC on Base). MPP family: one WWW-Authenticate: Payment\
  \ challenge per method (tempo, stripe,\n    card), Authorization: Payment on retry, Payment-Receipt on success. Reads (forms catalog, schemas, order\n    status) and validate endpoints are open.\n  note: 'The OpenAPI declares \"security\": [] at the top level and no components.securitySchemes — an accurate declaration of \"no authentication\", not an omission.'\n  sources: [openapi/postalform-com-machine-payments-openapi.json, https://postalform.com/agents]\n- name: none (MCP)\n  type: none\n  surface: MCP server (https://postalform.com/mcp) and its UCP (/ucp/mcp) and ACP (/acp/mcp) siblings\n  applied_to: initialize, tools/list, resources/list, read-only tools\n  gate_on_writes: 'hosted checkout_url (human pays on Stripe-hosted page); complete_checkout with a Stripe shared payment token (spt_..., provider stripe); postalform.create_machine_order 402 challenge retried with payment_authorization (MPP) or payment_signature (x402). UCP calls additionally require a platform profile in _meta.ucp.profile.'\n\
  \  rfc9728: 'not served — /.well-known/oauth-protected-resource 404 on the MCP host'\n  sources: [https://postalform.com/.well-known/mcp.json, https://postalform.com/developers, https://postalform.com/.well-known/capability-card.json]\nwebhook_verification:\n  header: PostalForm-Signature\n  secret: endpoint-scoped signing_secret, returned once on create/rotate\n  source: https://postalform.com/developer-mail-api (\"Verify the PostalForm-Signature header before trusting webhook payloads\")\n  note: The signature algorithm and header format are not documented publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postalform-com/refs/heads/main/authentication/postalform-com-authentication.yml
summary_line: http/none/payment-gated · 3 schemes
tags:
- Physical Mail
- Print & Mail
- Postal Mail
- Certified Mail
- Documents
- Agents
- Agentic Commerce
- MCP
- A2A
- x402
- Machine Payments
- Webhook
- agent-native
- United States
---
