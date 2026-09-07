---
anonymous_access: false
api_key_in: []
auth_types: []
description: Confido Legal authenticates every GraphQL request with a single API-key header. There is no OAuth 2.0, no OIDC, no mutual TLS and no scope system; authority is expressed by which of four token TYPES you hold, each identifiable from a human-readable prefix.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Confido Legal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Confido Legal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Confido Legal
provider_slug: confido-legal
scheme_count: 1
schemes:
- description: All four token types are presented in the same header.
  id: apiKey
  in: header
  name: x-api-key
  type: apiKey
slug: confido-legal-authentication
source_filename: confido-legal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.confidolegal.com/docs/introduction/authorization\nprovider: Confido Legal\nproviderId: confido-legal\ndescription: >-\n  Confido Legal authenticates every GraphQL request with a single API-key header. There is\n  no OAuth 2.0, no OIDC, no mutual TLS and no scope system; authority is expressed by which\n  of four token TYPES you hold, each identifiable from a human-readable prefix.\ndocs: https://docs.confidolegal.com/docs/introduction/authorization\nschemes:\n- id: apiKey\n  type: apiKey\n  in: header\n  name: x-api-key\n  description: All four token types are presented in the same header.\ntoken_types:\n- name: Partner Token\n  prefix: p_secret_\n  environment_encoded: true\n  audience: server-side only\n  issued_by: Confido Legal Partner Portal, Settings\n  purpose: >-\n    Create and manage Firms and Firm tokens. Used with createFirm, firmApiTokenCreate and\n    firmApiTokenExchangeCode.\n  never_expose_to_frontend:\
  \ true\n- name: Firm Token\n  prefix: f_secret_\n  environment_encoded: true\n  audience: server-side only\n  issued_by: firmApiTokenCreate or createFirm (called with a Partner token), or the Connect code exchange\n  purpose: The workhorse credential — most API operations run under a Firm token.\n  never_expose_to_frontend: true\n- name: Payment Session Token\n  prefix: pay_public_\n  environment_encoded: true\n  audience: browser / frontend\n  issued_by: paymentSessionCreate (Firm token required)\n  purpose: Initialize the Hosted Fields JavaScript SDK for one payment.\n  single_use: true\n- name: Onboarding Token\n  prefix: onboarding_public_\n  environment_encoded: true\n  audience: browser / frontend\n  issued_by: createOnboardingToken (Firm token required)\n  purpose: Initialize onboarding.js to render the firm application form.\n  short_lived: true\nprefix_semantics: >-\n  Tokens are self-describing. In \"p_secret_sandbox_…\" the leading segment names the token\n  type, \"secret\"\
  \ or \"public\" says whether it may reach a browser, and \"sandbox\" names the\n  environment. Sandbox and production tokens are not interchangeable.\nscopes:\n  supported: false\n  detail: >-\n    Confido states plainly that Firm API tokens are NOT scoped — there is no read-only\n    versus full-access token. Any valid Firm token can perform every Firm-level operation\n    the product allows server-side. There is consequently no scopes/ artifact for this\n    provider.\n  schema_note: >-\n    The schema does expose a `Scope` type (with ScopeFirm, ScopePartner and\n    ScopePaymentSession variants) returned by the `me` query. This identifies WHICH\n    principal a token represents, not a permission set.\nlifecycle:\n  expiry: >-\n    Firm tokens are long-lived — no TTL, no refresh endpoint, no rotate endpoint. Payment\n    Session tokens are single-use; Onboarding tokens are short-lived.\n  rotation: >-\n    Create a new token (firmApiTokenCreate), then revoke the old one in the Confido\
  \ Legal\n    app under Settings, API Tokens. Revocation takes effect immediately.\n  multiple_tokens: A Firm may hold more than one active token simultaneously.\n  revocation_notification: >-\n    No webhook fires when a Firm API token is created or revoked. Handle 401/403 responses\n    by checking the portal — there is no push signal to react to.\n  management_operations: [firmApiTokenCreate, firmApiTokenList, firmApiTokenUpdate, firmApiTokenDelete, firmApiTokenExchangeCode]\ndelegation:\n  mechanism: Connect\n  detail: >-\n    A partner obtains authority over an existing firm through a redirect flow shaped like\n    OAuth but not implementing it: the user is sent to the partner's unique Connect URL,\n    authorizes, and is redirected to the partner's Callback URL with a one-time-use `code`\n    and an opaque `state` passthrough. firmApiTokenExchangeCode swaps the code for a Firm\n    token using the Partner token.\n  docs: https://docs.confidolegal.com/docs/firm-onboarding/connect\n\
  \  note: >-\n    No token endpoint, no refresh token, no scope parameter and no PKCE — this is a\n    bespoke code exchange, not OAuth 2.0.\nobserved_failure:\n  probed: '2026-09-05'\n  request: 'POST https://api.gravity-legal.com/ with x-api-key: f_secret_sandbox_<invalid>'\n  http_status: 500\n  body: >-\n    {\"errors\":[{\"message\":\"Context creation failed: Invalid firm token.\",\n    \"extensions\":{\"code\":\"INTERNAL_SERVER_ERROR\"},\"code\":\"INTERNAL_SERVER_ERROR\",\"status\":500}]}\n  finding: >-\n    An invalid credential returns HTTP 500 with extensions.code INTERNAL_SERVER_ERROR, not\n    a 401 and not an auth-specific code. A client cannot distinguish a revoked token from a\n    server fault by status or code — only by parsing the message string.\nanonymous_surface:\n  detail: >-\n    Schema introspection and the `me` query answer without any x-api-key (me returns a\n    Scope typename). No business data is reachable anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confido-legal/refs/heads/main/authentication/confido-legal-authentication.yml
summary_line: 1 scheme
tags:
- Compliance
- Disbursements
- GraphQL
- IOLTA
- Law
- LawTech
- Legal
- Legal Technology
- Payments
- Trust Accounting
---
