---
api_key_in: []
auth_types:
- passkey
- email-otp
- oauth2
- signed-authorization
- delegated-session
description: ''
kind: authentication
layout: security
method: searched
name: Kite Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
overview: Kite secures its APIs with passkey, email-otp, oauth2, signed-authorization, and delegated-session across 8 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code flow(s).
provider_name: Kite
provider_slug: kite
scheme_count: 8
schemes:
- commands:
  - kpass signup init --email <EMAIL>
  - kpass signup poll --signup-id <SIGNUP_ID> --wait
  - kpass signup exchange --signup-id <SIGNUP_ID> --exchange-token <TOKEN>
  description: Signup sends an email verification link; the client polls for completion then exchanges a signup id plus exchange token for credentials.
  name: email-signup-verification
  source: https://docs.gokite.ai/kite-agent-passport/cli-reference
  type: email-link
- commands:
  - kpass login init --email <EMAIL>
  - kpass login verify --login-id <LOGIN_ID> --code <OTP_CODE>
  description: Login sends an 8-character one-time code by email, verified against a login id.
  name: email-otp-login
  source: https://docs.gokite.ai/kite-agent-passport/cli-reference
  type: otp
- description: Passkeys are the primary human authenticator. Sensitive actions - sending funds, approving agent sessions, adding or removing passkeys - require action-bound step-up re-confirmation. Account recovery runs over email with a one-click cancel link, passkey changes trigger email notifications, passkeys carry device names, and a first-passkey risk hold applies on enrollment.
  features:
  - action-bound step-up verification
  - account recovery flow
  - login and security-verification history (time, location, device)
  - step-up browser approval for wallet sends showing amount, asset, recipient, and sending wallet
  name: passkey
  source: https://docs.gokite.ai/changelog/2026/2026-06-04-backend-v1-3-0
  type: webauthn
- approval: explicit user approval, awaited via kpass agent:session status --request-id <ID> --wait
  description: The agent's credential is a user-approved spending session rather than a long-lived key. A session is bounded by max-amount-per-tx, max-total-amount (USD-denominated caps), a TTL, an allowed asset set, and a payment approach. Sessions can be attached, switched, listed, and have budgets edited.
  name: agent-spending-session
  parameters:
  - max-amount-per-tx
  - max-total-amount
  - ttl
  - assets
  - payment-approach
  source: https://docs.gokite.ai/kite-agent-passport/cli-reference
  type: delegated-authority
- description: Per-request payment proof presented as a base64-encoded signed authorization in the X-PAYMENT header, verified and settled by an x402 facilitator.
  encoding: base64
  header: X-PAYMENT
  name: x402-payment-authorization
  source: https://docs.gokite.ai/kite-agent-passport/service-provider-guide
  type: signed-authorization
- description: Gasless stablecoin transfers are authorized off-chain with an EIP-3009 signature (v, r, s) over a transferWithAuthorization payload carrying from, to, value, validAfter, validBefore, tokenAddress, and a single-use nonce. EIP-712 domain name and version per token are published by GET /supported_tokens.
  name: eip3009-transfer-authorization
  source: https://docs.gokite.ai/kite-chain/9-gasless-integration
  standard: EIP-3009
  type: signed-authorization
- description: The hosted Passport MCP endpoint authorizes MCP clients (ChatGPT and others) over OAuth before an agent may discover, pay, and manage sessions.
  flow: authorization_code
  name: mcp-oauth
  source: https://docs.gokite.ai/changelog/2026/2026-06-23-release
  type: oauth2
- description: Embed tokens for partner embedded flows are delivered via URL fragment and resolved with an X-Embed-Token request header (changed from a query parameter).
  header: X-Embed-Token
  name: partner-embed-token
  source: https://docs.gokite.ai/changelog/2026/2026-07-15-release
  type: token
slug: kite-authentication
source_filename: kite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.gokite.ai/kite-agent-passport/cli-reference\ndocs:\n- https://docs.gokite.ai/kite-agent-passport/cli-reference\n- https://docs.gokite.ai/changelog/2026/2026-06-04-backend-v1-3-0\n- https://docs.gokite.ai/kite-agent-passport/service-provider-guide\nderivation_note: >-\n  Derived by reading the published docs, not from an OpenAPI securitySchemes block - Kite publishes no\n  OpenAPI (its API Reference page is an explicit \"Coming soon\" placeholder). derive-authentication.py\n  would yield nothing for this repo.\nsummary:\n  types: [passkey, email-otp, oauth2, signed-authorization, delegated-session]\n  human_principal: passkey (WebAuthn) with email one-time code and email magic-link enrollment\n  agent_principal: delegated spending session bound to caps, TTL, assets, and payment protocol\n  value_transfer: EIP-3009 / x402 signed payment authorizations\n  api_key_in: []\n  oauth2_flows: [authorization_code]\nschemes:\n\
  - name: email-signup-verification\n  type: email-link\n  description: Signup sends an email verification link; the client polls for completion then exchanges a\n    signup id plus exchange token for credentials.\n  commands:\n  - kpass signup init --email <EMAIL>\n  - kpass signup poll --signup-id <SIGNUP_ID> --wait\n  - kpass signup exchange --signup-id <SIGNUP_ID> --exchange-token <TOKEN>\n  source: https://docs.gokite.ai/kite-agent-passport/cli-reference\n- name: email-otp-login\n  type: otp\n  description: Login sends an 8-character one-time code by email, verified against a login id.\n  commands:\n  - kpass login init --email <EMAIL>\n  - kpass login verify --login-id <LOGIN_ID> --code <OTP_CODE>\n  source: https://docs.gokite.ai/kite-agent-passport/cli-reference\n- name: passkey\n  type: webauthn\n  description: >-\n    Passkeys are the primary human authenticator. Sensitive actions - sending funds, approving agent\n    sessions, adding or removing passkeys - require action-bound\
  \ step-up re-confirmation. Account\n    recovery runs over email with a one-click cancel link, passkey changes trigger email notifications,\n    passkeys carry device names, and a first-passkey risk hold applies on enrollment.\n  features:\n  - action-bound step-up verification\n  - account recovery flow\n  - login and security-verification history (time, location, device)\n  - step-up browser approval for wallet sends showing amount, asset, recipient, and sending wallet\n  source: https://docs.gokite.ai/changelog/2026/2026-06-04-backend-v1-3-0\n- name: agent-spending-session\n  type: delegated-authority\n  description: >-\n    The agent's credential is a user-approved spending session rather than a long-lived key. A session is\n    bounded by max-amount-per-tx, max-total-amount (USD-denominated caps), a TTL, an allowed asset set,\n    and a payment approach. Sessions can be attached, switched, listed, and have budgets edited.\n  parameters:\n  - max-amount-per-tx\n  - max-total-amount\n\
  \  - ttl\n  - assets\n  - payment-approach\n  approval: explicit user approval, awaited via kpass agent:session status --request-id <ID> --wait\n  source: https://docs.gokite.ai/kite-agent-passport/cli-reference\n- name: x402-payment-authorization\n  type: signed-authorization\n  description: Per-request payment proof presented as a base64-encoded signed authorization in the\n    X-PAYMENT header, verified and settled by an x402 facilitator.\n  header: X-PAYMENT\n  encoding: base64\n  source: https://docs.gokite.ai/kite-agent-passport/service-provider-guide\n- name: eip3009-transfer-authorization\n  type: signed-authorization\n  description: >-\n    Gasless stablecoin transfers are authorized off-chain with an EIP-3009 signature (v, r, s) over a\n    transferWithAuthorization payload carrying from, to, value, validAfter, validBefore, tokenAddress,\n    and a single-use nonce. EIP-712 domain name and version per token are published by\n    GET /supported_tokens.\n  standard: EIP-3009\n\
  \  source: https://docs.gokite.ai/kite-chain/9-gasless-integration\n- name: mcp-oauth\n  type: oauth2\n  flow: authorization_code\n  description: The hosted Passport MCP endpoint authorizes MCP clients (ChatGPT and others) over OAuth\n    before an agent may discover, pay, and manage sessions.\n  source: https://docs.gokite.ai/changelog/2026/2026-06-23-release\n- name: partner-embed-token\n  type: token\n  description: Embed tokens for partner embedded flows are delivered via URL fragment and resolved with\n    an X-Embed-Token request header (changed from a query parameter).\n  header: X-Embed-Token\n  source: https://docs.gokite.ai/changelog/2026/2026-07-15-release\nscopes:\n  documented: false\n  note: >-\n    A scope-prefix matching fix in the 2026-07-15 release confirms an internal scope model exists, but no\n    public scope or permission reference is published. scopes/ is intentionally not emitted rather than\n    invented.\nrelated:\n- conventions/kite-conventions.yml\n- cli/kite-cli.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kite/refs/heads/main/authentication/kite-authentication.yml
summary_line: passkey/email-otp/oauth2/signed-authorization/delegated-session · 8 schemes
tags:
- Agentic Payments
- AI Agents
- x402
- Stablecoins
- Blockchain
- EVM
- Layer 1
- Machine-to-Machine
- Identity
- Payments
- JSON-RPC
- Account Abstraction
---
