---
api_key_in: []
api_specs:
- filename: api-for-ai.yaml
  format: yaml
  label: Wealth Reader API
  slug: wealth-reader-api
  spec_type: OpenAPI
  url: https://www.wealthreader.com/api-reference/api-for-ai.yaml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Wealth Reader Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wealth Reader declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Wealth Reader
provider_slug: wealth-reader
scheme_count: 5
schemes:
- applies_to: every operation except GET /entities/ and GET /error-codes/ (public catalogue reads)
  id: api_key
  in: formData
  name: api_key
  note: Also accepted as a query parameter on GET /cards/transactions/, where the spec itself warns "it travels in the query string, so it ends up in access logs and intermediary proxies". api.wealthreader.com advertises X-API-KEY in Access-Control-Allow-Headers, so a header form exists at the edge, but the published operations use the form field.
  obtained_from: signup plus an onboarding session with the technical team
  transport: application/x-www-form-urlencoded request body
  type: apiKey
- applies_to: POST /entities/, POST /tokens/revoke/, POST /tokens/reasign/
  description: Opaque handle to the end user's custodied bank credential, returned in statistics.token the first time credentials are tokenized. Reusable for later refreshes; invalidated when the user changes their password or the bank raises a new second factor, which surfaces as error code 3 (blocked token) or 4 (temporarily invalid).
  id: bank_token
  lifecycle:
    issue: tokenize=1 on the widget or the domain registration
    list: POST /tokens/ (operationId queryTokensByApiKey), 500 per page
    reassign: POST /tokens/reasign/ (operationId reasignToken) — moves a token between api_keys
    revoke: POST /tokens/revoke/ (operationId revokeToken)
  name: token
  type: custodied_credential
- authorization_endpoint: https://oauth.wealthreader.com/oauth2/
  grant: authorization_code with PKCE (S256)
  id: oauth_pkce
  note: 'Shaped like OAuth 2.0 + PKCE — response_type=code, code_challenge_method=S256, state, nonce, redirect_uri, and a code exchanged at /token/ — but it is NOT standards-discoverable and it is not the standard flow. There is no /.well-known/oauth-authorization-server (probed 404 on both hosts) and no /.well-known/openid-configuration. No scopes are defined. Parameter names differ from RFC 7636: the challenge is sent as `challenge_code`, not `code_challenge`. The docs require the verifier to be a 41-character alphanumeric string hex-encoded to 82 characters, and `wr_conf` (the selector configuration JSON) is hex-encoded into the query string. Used when the integrator cannot embed the iframe — native apps and redirect flows.'
  scopes: []
  token_endpoint: https://oauth.wealthreader.com/token/
  type: oauth2-like
- algorithm: sha256=<hex of hmac_sha256(raw_body, webhook_secret)>
  applies_to: real-time cards webhook deliveries
  header: X-WR-Signature
  id: webhook_signature
  secret_issuance: 64 hex characters, returned exactly once by POST /cards/webhook/ on first setup or when rotate_secret is true; otherwise it comes back null and cannot be retrieved again.
  type: hmac
  verification: The provider explicitly instructs consumers to compare in constant time (hash_equals or equivalent) before trusting the body.
- env: ALLWR_TOOLKIT_ALLWR_API_KEY
  id: allwr_api_key
  key_prefix: wrk_
  note: The only scoped credential anywhere in the company's published surface. Created under Settings -> API keys in an ALL WR workspace. Recorded because it is the only place the provider documents a named permission scope.
  product: ALL WR (allwr.io) — sibling platform, not the bank-aggregation API
  scope: tasks:import
  source: https://raw.githubusercontent.com/Wealth-Reader/allwr-toolkit/main/docs/authentication.md
  type: apiKey
slug: wealth-reader-authentication
source_filename: wealth-reader-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: >-\n  https://www.wealthreader.com/docs/en/iframe-integration-2-of-2-backend.md ;\n  https://www.wealthreader.com/docs/en/oauth-integration-backend.md ;\n  openapi/wealth-reader-api-for-ai.yaml ; live response headers from https://api.wealthreader.com/entities/\ndocs: https://www.wealthreader.com/docs/en/oauth-integration-backend/\nsummary: >-\n  Two-layer auth. The CLIENT authenticates to Wealth Reader with a static api_key. The END USER\n  authenticates to their own bank inside Wealth Reader's widget or OAuth flow, and the result of\n  that is a reusable `token` that Wealth Reader custodies on the client's behalf. The OpenAPI\n  declares NO securitySchemes at all — the api_key travels as an ordinary form field — so nothing\n  in the machine-readable contract tells a client generator that these calls are authenticated.\nspec_declares_security: false\nschemes:\n- id: api_key\n  type: apiKey\n  in: formData\n  name: api_key\n\
  \  transport: application/x-www-form-urlencoded request body\n  applies_to: every operation except GET /entities/ and GET /error-codes/ (public catalogue reads)\n  note: >-\n    Also accepted as a query parameter on GET /cards/transactions/, where the spec itself warns\n    \"it travels in the query string, so it ends up in access logs and intermediary proxies\".\n    api.wealthreader.com advertises X-API-KEY in Access-Control-Allow-Headers, so a header form\n    exists at the edge, but the published operations use the form field.\n  obtained_from: signup plus an onboarding session with the technical team\n- id: bank_token\n  type: custodied_credential\n  name: token\n  applies_to: 'POST /entities/, POST /tokens/revoke/, POST /tokens/reasign/'\n  description: >-\n    Opaque handle to the end user's custodied bank credential, returned in statistics.token the\n    first time credentials are tokenized. Reusable for later refreshes; invalidated when the user\n    changes their password or\
  \ the bank raises a new second factor, which surfaces as error code 3\n    (blocked token) or 4 (temporarily invalid).\n  lifecycle:\n    issue: tokenize=1 on the widget or the domain registration\n    revoke: 'POST /tokens/revoke/ (operationId revokeToken)'\n    reassign: 'POST /tokens/reasign/ (operationId reasignToken) — moves a token between api_keys'\n    list: 'POST /tokens/ (operationId queryTokensByApiKey), 500 per page'\n- id: oauth_pkce\n  type: oauth2-like\n  authorization_endpoint: https://oauth.wealthreader.com/oauth2/\n  token_endpoint: https://oauth.wealthreader.com/token/\n  grant: authorization_code with PKCE (S256)\n  scopes: []\n  note: >-\n    Shaped like OAuth 2.0 + PKCE — response_type=code, code_challenge_method=S256, state, nonce,\n    redirect_uri, and a code exchanged at /token/ — but it is NOT standards-discoverable and it is\n    not the standard flow. There is no /.well-known/oauth-authorization-server (probed 404 on both\n    hosts) and no /.well-known/openid-configuration.\
  \ No scopes are defined. Parameter names differ\n    from RFC 7636: the challenge is sent as `challenge_code`, not `code_challenge`. The docs\n    require the verifier to be a 41-character alphanumeric string hex-encoded to 82 characters, and\n    `wr_conf` (the selector configuration JSON) is hex-encoded into the query string. Used when the\n    integrator cannot embed the iframe — native apps and redirect flows.\n- id: webhook_signature\n  type: hmac\n  header: X-WR-Signature\n  algorithm: 'sha256=<hex of hmac_sha256(raw_body, webhook_secret)>'\n  applies_to: real-time cards webhook deliveries\n  secret_issuance: >-\n    64 hex characters, returned exactly once by POST /cards/webhook/ on first setup or when\n    rotate_secret is true; otherwise it comes back null and cannot be retrieved again.\n  verification: >-\n    The provider explicitly instructs consumers to compare in constant time (hash_equals or\n    equivalent) before trusting the body.\n- id: allwr_api_key\n  type: apiKey\n\
  \  product: ALL WR (allwr.io) — sibling platform, not the bank-aggregation API\n  key_prefix: wrk_\n  scope: 'tasks:import'\n  env: ALLWR_TOOLKIT_ALLWR_API_KEY\n  source: https://raw.githubusercontent.com/Wealth-Reader/allwr-toolkit/main/docs/authentication.md\n  note: >-\n    The only scoped credential anywhere in the company's published surface. Created under\n    Settings -> API keys in an ALL WR workspace. Recorded because it is the only place the\n    provider documents a named permission scope.\ncallback_auth:\n  mechanism: none\n  detail: >-\n    The iframe callback POST to the integrator's own HTTPS endpoint carries no signature and no\n    shared secret — only the operation_id the integrator generated. Authenticity rests on the\n    integrator having registered that domain and callback URL in the client area beforehand, and\n    on the operation_id being unguessable. The integrator must answer HTTP 200 with\n    {\"status\":\"ok\"} or the widget will not report success to the\
  \ frontend. Contrast with the cards\n    webhook, which IS HMAC-signed.\ngaps:\n- The OpenAPI declares no securitySchemes, so generated clients get no auth wiring.\n- No OAuth discovery document; no scopes; non-standard PKCE parameter names.\n- The iframe callback is unsigned.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server (both 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealth-reader/refs/heads/main/authentication/wealth-reader-authentication.yml
summary_line: 5 schemes
tags:
- Bank Aggregation
- Open Banking
- PSD2
- Financial Data
- Account Aggregation
- Investment Portfolios
- Wealth Management
- Banking
- Fintech
---
