---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nav Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nav secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nav
provider_slug: nav
scheme_count: 2
schemes:
- applies_to: All nine Nav Partner API operations under https://api.nav.com/v1
  errors:
  - meaning: API key is missing or invalid.
    status: 401
  - meaning: API key is valid but the operation is not permitted for this partner.
    status: 403
  example_header: 'Authorization: Bearer <api_key>'
  in: header
  name: PartnerApiKey
  parameter_name: Authorization
  provisioning: '"API keys are provisioned by Nav during partner onboarding. Contact your Nav account manager to obtain, rotate, or revoke a key." There is no developer console, no self-serve key issuance and no documented programmatic rotation.'
  rotation: manual, via Nav account manager
  scheme_note: 'Documented as `Type: apiKey`, `Header: Authorization` with the value `Bearer <api_key>`. It is a static bearer token, not an OAuth 2.0 access token — there is no authorization server, no token endpoint, no scopes and no refresh.'
  source: https://api-docs.nav.com/docs/rest-api/auth/partner-api-key
  type: apiKey
- additional_headers:
  - description: Partner ID, provided by Nav.
    name: x-partner-id
  in: header
  name: PartnerApiKeyLegacyGraphQL
  parameter_name: x-api-key
  scheme_note: 'The deprecated GraphQL API used a different scheme: `x-api-key` plus an `x-partner-id` header. Recorded for partners still on the legacy integration; the GraphQL endpoint documented at https://api.nav.com/partners/graphql returned HTTP 404 when probed 2026-08-26 and the sandbox equivalent returned 503.'
  source: https://api-docs.nav.com/docs/deprecated/graphql-schema
  status: deprecated
  type: apiKey
slug: nav-authentication
source_filename: nav-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://api-docs.nav.com/docs/rest-api/auth/partner-api-key\ndocs: https://api-docs.nav.com/docs/rest-api/auth/partner-api-key\nchecked: '2026-08-26'\nderivation_note: >-\n  Not derived by derive-authentication.py — Nav publishes no OpenAPI, so there are no\n  securitySchemes to read. Every field below is transcribed from the published authentication and\n  widget documentation.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  self_serve_credentials: false\nschemes:\n- name: PartnerApiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  scheme_note: >-\n    Documented as `Type: apiKey`, `Header: Authorization` with the value `Bearer <api_key>`. It is a\n    static bearer token, not an OAuth 2.0 access token — there is no authorization server, no token\n    endpoint, no scopes and no refresh.\n  example_header: 'Authorization: Bearer <api_key>'\n\
  \  applies_to: All nine Nav Partner API operations under https://api.nav.com/v1\n  provisioning: >-\n    \"API keys are provisioned by Nav during partner onboarding. Contact your Nav account manager to\n    obtain, rotate, or revoke a key.\" There is no developer console, no self-serve key issuance and\n    no documented programmatic rotation.\n  rotation: manual, via Nav account manager\n  errors:\n  - status: 401\n    meaning: API key is missing or invalid.\n  - status: 403\n    meaning: API key is valid but the operation is not permitted for this partner.\n  source: https://api-docs.nav.com/docs/rest-api/auth/partner-api-key\n- name: PartnerApiKeyLegacyGraphQL\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  status: deprecated\n  scheme_note: >-\n    The deprecated GraphQL API used a different scheme: `x-api-key` plus an `x-partner-id` header.\n    Recorded for partners still on the legacy integration; the GraphQL endpoint documented at\n    https://api.nav.com/partners/graphql\
  \ returned HTTP 404 when probed 2026-08-26 and the sandbox\n    equivalent returned 503.\n  additional_headers:\n  - name: x-partner-id\n    description: Partner ID, provided by Nav.\n  source: https://api-docs.nav.com/docs/deprecated/graphql-schema\nbrowser_session_model:\n  name: Widget init token\n  kind: single-use bearer token, browser-delivered\n  minted_by: POST /v1/sso-token (server-side, with the partner API key)\n  lifetime_seconds: 120\n  single_use: true\n  delivery: >-\n    The partner's own backend authenticates its user, calls POST /v1/sso-token with that user's Nav\n    accountId, and returns ONLY the token to the browser. The token is passed to the\n    <nav-credit-widget> custom element via the `token` attribute or provideToken() in response to\n    the navWidgetTokenRequest event.\n  hard_rule_from_docs: >-\n    \"The API key must never appear in browser code.\" Nav states this explicitly and the widget\n    architecture enforces it — the widget runs in a cross-origin\
  \ iframe so Nav data never enters the\n    partner's JavaScript context.\n  additional_control: >-\n    Widget-bearing origins must be registered with Nav before production. The allow list is itself\n    an API surface (GET/PUT /v1/origins) and supports exact origins plus single-level wildcards\n    (https://*.example.com matches one subdomain label only).\n  reuse_failure_mode: >-\n    Reusing a cached init token causes the widget to terminate with a SESSION_ERROR after a failed\n    session exchange. See errors/nav-error-codes.yml.\n  source: https://api-docs.nav.com/docs/widgets/getting-started\ngaps:\n  oauth2: >-\n    No OAuth 2.0 or OpenID Connect anywhere on the Nav surface. No /.well-known/oauth-authorization-server,\n    no /.well-known/openid-configuration (all 404 — see well-known/nav-well-known.yml). scopes/ is\n    therefore not emitted for this provider: a static bearer key has no scope surface, and an empty\n    OAuthScopes artifact would be a fabrication.\n  key_prefix:\
  \ >-\n    Nav does not publish a key prefix convention (no lp_/sk_test_ style discriminator), so a partner\n    cannot tell a sandbox key from a production key by inspection. The environment is selected by\n    base URL (api.nav.com vs api.sandbox.nav.com), not by the credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nav/refs/heads/main/authentication/nav-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Business Credit
- Small Business
- Financial Services
- Embedded Finance
- Lending
- Credit Scores
- Credit Reporting
- Financing Marketplace
- Fintech
- Partner API
---
