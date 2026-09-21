---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getvda-ai-witness-openapi.json
  format: json
  label: VDA Witness API
  slug: vda-witness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-witness-openapi.json
- filename: getvda-ai-hitl-openapi.json
  format: json
  label: VDA HITL API
  slug: vda-hitl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-hitl-openapi.json
- filename: getvda-ai-acp-openapi.json
  format: json
  label: VDA ACP API
  slug: vda-acp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-acp-openapi.json
- filename: getvda-ai-c2md-edge-openapi.json
  format: json
  label: C2MD Compliance Agent
  slug: c2md-compliance-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-c2md-edge-openapi.json
- filename: getvda-ai-gosce-router-openapi.json
  format: json
  label: GOSCE Agent Portfolio and Router
  slug: gosce-agent-portfolio-and-router
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-gosce-router-openapi.json
auth_types:
- http
- oauth2
- x402-payment
description: ''
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: Getvda Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verified Digital Agents (VDA) secures its APIs with http, oauth2, and x402-payment across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Verified Digital Agents (VDA)
provider_slug: getvda-ai
scheme_count: 7
schemes:
- aka: witness_bearer / bearerAuth (HITL) — the same credential under three scheme names
  alternate_header: x-witness-key
  bearerFormat: wtn.<keyId>.<secret>
  issued_by: POST https://witness.getvda.ai/api/witness/test-key (self-serve, instant, no human) — also the MCP tool get_test_key and the card's provisioning.selfServeKey
  name: witnessApiKey
  public_exceptions:
  - POST /api/witness/verify
  - GET /api/witness/credentials/{credential_id}
  - GET /api/witness/records/{recordId}/issuer
  - POST /api/witness/test-key
  - renew/challenge + renew (controller signature instead)
  - MCP initialize/tools/list on Witness and C2MD
  - ACP GET /bundles/*
  renewal: POST /api/witness/renew/challenge -> Ed25519-sign sign_payload "vda.witness.renew/1|<accountId>|<nonce>" with the bound controller key -> POST /api/witness/renew; prior keys stay valid until expiry
  revocation: POST /api/witness/keys/revoke — total and itself sealed as a key_revocation event
  scheme: bearer
  sources:
  - openapi/getvda-ai-witness-openapi.json
  - openapi/getvda-ai-hitl-openapi.json
  - openapi/getvda-ai-acp-openapi.json
  - a2a/getvda-ai-c2md-agent-card.json
  type: http
  used_by:
  - witness.getvda.ai
  - hitl.getvda.ai (every method incl. MCP initialize)
  - acp.getvda.ai (/v1 routes)
  - c2md.getvda.ai (generative tools; account tier maps to c2md:* scopes)
  validation: siblings call GET /api/witness/whoami -> {account_id, tier SEALED|ANCHORED, scopes [seal, read], compliance, key_id, revoked, expires_at}; 200 is Cache-Control private max-age=60, 401 is generic + no-store
- description: 'Not a request credential but the root of the account: an Ed25519 public JWK ({kty OKP, crv Ed25519, x}) bound at mint time or via POST /api/witness/account/bind-controller. Authorises key renewal and controller-signed key revocation; "there is no standing credential to leak". Distinct from the record-signing key (customer-managed custody, published at the issuer''s did:web) and the did:web card-signing key — the docs call out THREE keys.'
  name: controllerKey
  scheme: Ed25519 challenge-response
  sources:
  - https://witness.getvda.ai/llms.txt
  type: signature
- description: Google Sign-In for Workspace and personal accounts; token validated via Google's JWKS; used for C2MD skill-tier scope assertion against subscription state.
  flows:
    authorizationCode:
      authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
      scopes:
      - c2md:assess
      - c2md:generate_starter
      - c2md:generate_pro
      - c2md:generate_journey
      - c2md:commercial_deploy
      tokenUrl: https://oauth2.googleapis.com/token
  name: google_oauth2
  sources:
  - a2a/getvda-ai-c2md-agent-card.json
  type: oauth2
  used_by:
  - c2md.getvda.ai
- description: Microsoft Entra ID, organisations only (personal accounts unsupported); clientCredentials is for pre-registered service principals (Tier 3, by arrangement — hello@getvda.ai).
  flows:
    authorizationCode:
      authorizationUrl: https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize
      scopes:
      - c2md:assess
      - c2md:generate_starter
      - c2md:generate_pro
      - c2md:generate_journey
      - c2md:commercial_deploy
      tokenUrl: https://login.microsoftonline.com/organizations/oauth2/v2.0/token
    clientCredentials:
      scopes:
      - 7c89fa90-05ca-4779-8128-32c7f11f604b/.default
      tokenUrl: https://login.microsoftonline.com/organizations/oauth2/v2.0/token
  name: microsoft_oauth2
  sources:
  - a2a/getvda-ai-c2md-agent-card.json
  type: oauth2
  used_by:
  - c2md.getvda.ai
- description: An OIDC token from the customer's IdP identifying a human approver on ACP's decision route. DECLARED but not live — GET https://acp.getvda.ai/readyz reports identity "disabled" ("set OIDC_ISSUER + OIDC_AUDIENCE to enable").
  header: X-Approver-Credential
  in: header
  name: approver_oidc
  scheme: bearer
  sources:
  - a2a/getvda-ai-acp-agent-card.json
  - openapi/getvda-ai-acp-openapi.json
  status: staged
  type: http
  used_by:
  - acp.getvda.ai
- description: Per-tenant service-account token for the Onboarding agent's admit_agent, revoke_credential and get_admission_status skills.
  name: tenantBearer
  scheme: bearer
  sources:
  - a2a/getvda-ai-onboard-agent-card.json
  type: http
  used_by:
  - onboard.getvda.ai
- description: The GOSCE fleet (98 servers + router) requires NO authentication; metered tools answer 402 with a base64 PAYMENT-REQUIRED header and are retried with a PAYMENT-SIGNATURE header — an EIP-3009 transferWithAuthorization in USDC on Base (eip155:8453) or an nvm:card-delegation Stripe checkout for humans. The C2MD card notes generated Copilot Studio connectors are "remote streamable-HTTP MCP servers requiring NO authentication".
  name: x402
  scheme: x402 v2 (HTTP 402 challenge)
  sources:
  - well-known/getvda-ai-agents-ai-catalog.json
  - https://agents.getvda.ai/llms.txt
  type: payment
  used_by:
  - '*.getvda.ai fleet'
  - router.getvda.ai
slug: getvda-ai-authentication
source_filename: getvda-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://witness.getvda.ai/llms.txt\nderived_from:\n- openapi/getvda-ai-witness-openapi.json\n- openapi/getvda-ai-hitl-openapi.json\n- openapi/getvda-ai-acp-openapi.json\n- a2a/getvda-ai-c2md-agent-card.json\n- a2a/getvda-ai-onboard-agent-card.json\n- well-known/getvda-ai-agents-ai-catalog.json\ndocs:\n- https://witness.getvda.ai/docs\n- https://witness.getvda.ai/llms.txt\n- https://c2md.getvda.ai/llms.txt\n- https://agents.getvda.ai/llms.txt\nsummary:\n  types: [http, oauth2, x402-payment]\n  model: >-\n    One suite credential minted by Witness and validated everywhere else through Witness GET /whoami (\"Contract A\"):\n    `Authorization: Bearer wtn.<keyId>.<secret>`. Witness also accepts the same key in an `x-witness-key` header. The\n    key is short-lived by design (quick-start keys expire in 7 days) and is renewed unattended by Ed25519\n    controller-key challenge-response, so the durable identity is the account (acct_<ULID>)\
  \ plus a controller key\n    the caller holds, not a standing secret. There is no OAuth authorization server on any VDA host; C2MD delegates\n    human sign-in to Google and Microsoft Entra, ACP declares an OIDC approver credential it does not yet enforce\n    (readyz: identity disabled), Onboarding uses a per-tenant bearer, and the GOSCE fleet has no authentication at\n    all — execution is gated by x402 payment.\n  observed:\n  - {request: 'POST https://witness.getvda.ai/api/witness/seal (no header)', status: 401, body: '{\"error\":\"unknown or invalid API key\"}'}\n  - {request: 'POST https://hitl.getvda.ai/mcp (no header)', status: 401, body: '{\"error\":\"unauthorized\",\"message\":\"missing bearer credential\"}'}\n  - {request: 'POST https://witness.getvda.ai/api/witness/mcp tools/list (no header)', status: 200, note: discovery is anonymous}\nschemes:\n- name: witnessApiKey\n  aka: witness_bearer / bearerAuth (HITL) — the same credential under three scheme names\n  type: http\n\
  \  scheme: bearer\n  bearerFormat: wtn.<keyId>.<secret>\n  alternate_header: x-witness-key\n  issued_by: 'POST https://witness.getvda.ai/api/witness/test-key (self-serve, instant, no human) — also the MCP tool get_test_key and the card''s provisioning.selfServeKey'\n  renewal: 'POST /api/witness/renew/challenge -> Ed25519-sign sign_payload \"vda.witness.renew/1|<accountId>|<nonce>\" with the bound controller key -> POST /api/witness/renew; prior keys stay valid until expiry'\n  revocation: 'POST /api/witness/keys/revoke — total and itself sealed as a key_revocation event'\n  validation: 'siblings call GET /api/witness/whoami -> {account_id, tier SEALED|ANCHORED, scopes [seal, read], compliance, key_id, revoked, expires_at}; 200 is Cache-Control private max-age=60, 401 is generic + no-store'\n  used_by:\n  - witness.getvda.ai\n  - hitl.getvda.ai (every method incl. MCP initialize)\n  - acp.getvda.ai (/v1 routes)\n  - 'c2md.getvda.ai (generative tools; account tier maps to c2md:* scopes)'\n\
  \  public_exceptions:\n  - 'POST /api/witness/verify'\n  - 'GET /api/witness/credentials/{credential_id}'\n  - 'GET /api/witness/records/{recordId}/issuer'\n  - 'POST /api/witness/test-key'\n  - 'renew/challenge + renew (controller signature instead)'\n  - 'MCP initialize/tools/list on Witness and C2MD'\n  - 'ACP GET /bundles/*'\n  sources: [openapi/getvda-ai-witness-openapi.json, openapi/getvda-ai-hitl-openapi.json, openapi/getvda-ai-acp-openapi.json, a2a/getvda-ai-c2md-agent-card.json]\n- name: controllerKey\n  type: signature\n  scheme: Ed25519 challenge-response\n  description: >-\n    Not a request credential but the root of the account: an Ed25519 public JWK ({kty OKP, crv Ed25519, x}) bound at\n    mint time or via POST /api/witness/account/bind-controller. Authorises key renewal and controller-signed key\n    revocation; \"there is no standing credential to leak\". Distinct from the record-signing key (customer-managed\n    custody, published at the issuer's did:web) and the did:web\
  \ card-signing key — the docs call out THREE keys.\n  sources: [https://witness.getvda.ai/llms.txt]\n- name: google_oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n      tokenUrl: https://oauth2.googleapis.com/token\n      scopes: [c2md:assess, c2md:generate_starter, c2md:generate_pro, c2md:generate_journey, c2md:commercial_deploy]\n  description: Google Sign-In for Workspace and personal accounts; token validated via Google's JWKS; used for C2MD skill-tier scope assertion against subscription state.\n  used_by: [c2md.getvda.ai]\n  sources: [a2a/getvda-ai-c2md-agent-card.json]\n- name: microsoft_oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize\n      tokenUrl: https://login.microsoftonline.com/organizations/oauth2/v2.0/token\n      scopes: [c2md:assess, c2md:generate_starter, c2md:generate_pro, c2md:generate_journey,\
  \ c2md:commercial_deploy]\n    clientCredentials:\n      tokenUrl: https://login.microsoftonline.com/organizations/oauth2/v2.0/token\n      scopes: ['7c89fa90-05ca-4779-8128-32c7f11f604b/.default']\n  description: Microsoft Entra ID, organisations only (personal accounts unsupported); clientCredentials is for pre-registered service principals (Tier 3, by arrangement — hello@getvda.ai).\n  used_by: [c2md.getvda.ai]\n  sources: [a2a/getvda-ai-c2md-agent-card.json]\n- name: approver_oidc\n  type: http\n  scheme: bearer\n  in: header\n  header: X-Approver-Credential\n  description: An OIDC token from the customer's IdP identifying a human approver on ACP's decision route. DECLARED but not live — GET https://acp.getvda.ai/readyz reports identity \"disabled\" (\"set OIDC_ISSUER + OIDC_AUDIENCE to enable\").\n  used_by: [acp.getvda.ai]\n  status: staged\n  sources: [a2a/getvda-ai-acp-agent-card.json, openapi/getvda-ai-acp-openapi.json]\n- name: tenantBearer\n  type: http\n  scheme: bearer\n \
  \ description: Per-tenant service-account token for the Onboarding agent's admit_agent, revoke_credential and get_admission_status skills.\n  used_by: [onboard.getvda.ai]\n  sources: [a2a/getvda-ai-onboard-agent-card.json]\n- name: x402\n  type: payment\n  scheme: x402 v2 (HTTP 402 challenge)\n  description: >-\n    The GOSCE fleet (98 servers + router) requires NO authentication; metered tools answer 402 with a base64\n    PAYMENT-REQUIRED header and are retried with a PAYMENT-SIGNATURE header — an EIP-3009 transferWithAuthorization\n    in USDC on Base (eip155:8453) or an nvm:card-delegation Stripe checkout for humans. The C2MD card notes\n    generated Copilot Studio connectors are \"remote streamable-HTTP MCP servers requiring NO authentication\".\n  used_by: ['*.getvda.ai fleet', router.getvda.ai]\n  sources: [well-known/getvda-ai-agents-ai-catalog.json, https://agents.getvda.ai/llms.txt]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/authentication/getvda-ai-authentication.yml
summary_line: http/oauth2/x402-payment · 7 schemes
tags:
- Company
- AI Agents
- AI Governance
- Compliance
- Audit Trail
- Agent Identity
- A2A
- MCP
- x402
- EU AI Act
- Human-in-the-Loop
---
