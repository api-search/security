---
api_key_in:
- cookie
api_specs:
- filename: openapi.json
  format: json
  label: SignSealShip Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://docs.signsealship.com/api-reference/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Signsealship Authentication
name_suffix: Authentication
oauth_flows: []
overview: SignSealShip Partner API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SignSealShip Partner API
provider_slug: signsealship
scheme_count: 2
schemes:
- bearerFormat: sss_pk_...
  description: 'Partner API key. Send as `Authorization: Bearer sss_pk_...`.'
  display: shown to the holder exactly once, at issue, by email
  env_var: SIGNSEALSHIP_PARTNER_KEY
  env_var_source: https://signsealship.com/.well-known/api-onboarding.json
  header: Authorization
  key_format:
    entropy: 256 bits after the prefix, lowercase base32
    prefix: sss_pk_
    prefix_rationale: Stated in the docs -- the prefix makes a leaked key recognizable in logs and secret scanners.
    test_prefix: sss_pk_test_
  name: partnerKey
  scheme: bearer
  sources:
  - openapi/signsealship-partner-api-openapi.yml
  - https://docs.signsealship.com/api-reference/authentication
  storage: SHA-256 hash only; the raw key is never stored and cannot be recovered
  type: http
- cookie_prefix_note: The __Host- prefix is a real hardening choice -- it forces Secure, host-only scope and a path of /, so the cookie cannot be set by a subdomain.
  description: SignSealShip dashboard login session cookie. Accepted by the /api/partner/webhooks management routes as an alternative to the partner key.
  in: cookie
  name: sessionCookie
  parameter: __Host-session
  rate_limit: partner-portal, 120/min per session
  sources:
  - openapi/signsealship-partner-api-openapi.yml
  type: apiKey
slug: signsealship-authentication
source_filename: signsealship-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: >-\n  https://docs.signsealship.com/api-reference/authentication (docs) reconciled against\n  openapi/signsealship-partner-api-openapi.yml (contract) and\n  https://signsealship.com/.well-known/api-onboarding.json (onboarding descriptor)\ndocs: https://docs.signsealship.com/api-reference/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: partnerKey\n  type: http\n  scheme: bearer\n  bearerFormat: sss_pk_...\n  header: Authorization\n  description: 'Partner API key. Send as `Authorization: Bearer sss_pk_...`.'\n  key_format:\n    prefix: sss_pk_\n    test_prefix: sss_pk_test_\n    entropy: 256 bits after the prefix, lowercase base32\n    prefix_rationale: >-\n      Stated in the docs -- the prefix makes a leaked key recognizable in logs and secret\n      scanners.\n  storage: SHA-256 hash only; the raw key is never\
  \ stored and cannot be recovered\n  display: shown to the holder exactly once, at issue, by email\n  env_var: SIGNSEALSHIP_PARTNER_KEY\n  env_var_source: https://signsealship.com/.well-known/api-onboarding.json\n  sources:\n  - openapi/signsealship-partner-api-openapi.yml\n  - https://docs.signsealship.com/api-reference/authentication\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: __Host-session\n  description: >-\n    SignSealShip dashboard login session cookie. Accepted by the /api/partner/webhooks\n    management routes as an alternative to the partner key.\n  cookie_prefix_note: >-\n    The __Host- prefix is a real hardening choice -- it forces Secure, host-only scope and a path\n    of /, so the cookie cannot be set by a subdomain.\n  rate_limit: partner-portal, 120/min per session\n  sources:\n  - openapi/signsealship-partner-api-openapi.yml\nanonymous_surface:\n  operations: 8\n  detail: >-\n    Eight read operations require no credential at all: the public room\
  \ view, Closing Passport\n    verification and certificate download, and Proof Passport verification and document download.\n    POST /api/partner/request is also public and unauthenticated.\n  authorization_model: >-\n    Possession of the code IS the authorization. Room codes (40 hex), order codes and verify codes\n    (26 base32, 128 bits) are bearer credentials, not merely identifiers. They resolve one\n    SignSealShip-issued record and cannot be used for arbitrary querying -- an unknown code returns\n    404 {\"verdict\": \"unknown\"}, identical to a malformed one.\nissuance:\n  self_serve: true\n  endpoint: POST https://signsealship.com/api/partner/request\n  endpoint_auth: anonymous\n  rate_limit: partner-request, 5 per hour per IP\n  flow:\n  - Submit firm name, work email, role, expected volume and intended use case.\n  - >-\n    A business email domain plus a coherent, on-topic use case is issued a trial key instantly.\n    Anything else is queued for human review.\n  - The\
  \ raw key is emailed to the submitted work address, once.\n  agent_blocker: >-\n    BOTH OUTCOMES RETURN HTTP 200. The status code does not distinguish an instant issue from a\n    queued review, and the key never appears in the response body -- only in an email. An agent\n    cannot complete onboarding end to end without reading a mailbox. The provider names this\n    itself in the gaps[] list of its own /.well-known/api-onboarding.json, alongside the absence\n    of RFC 7591 dynamic client registration.\n  console: https://signsealship.com/partner/settings/keys\nrotation:\n  api_keys:\n    self_serve: false\n    mechanism: >-\n      NO self-serve key-rotation endpoint exists. To rotate -- routinely or after a suspected leak\n      -- contact SignSealShip; a replacement is issued and the old key deactivated. Deactivation\n      is immediate once actioned, but it is a human step.\n    gap: >-\n      This is the weakest link in an otherwise careful credential design. A hashed, prefixed,\n\
  \      once-displayed key is good practice; requiring a human email to rotate it is not, and it\n      means incident response has a person in the critical path.\n  room_links:\n    self_serve: true\n    operation: POST /api/rooms/{roomCode}/rotate\n    effect: Every previously shared link dies instantly. Irreversible.\n  webhook_secrets:\n    self_serve: true\n    operation: POST /api/partner/webhooks/{id}/rotate\n    display: shown exactly once; only the hash is stored\n    overlap: >-\n      24 hours of dual signing -- the SignSealShip-Signature header carries one v1 entry per\n      active secret, and a consumer should accept when ANY entry matches. The machine-readable\n      form is previousSecretExpiresAt on RotateWebhookResponse.\nauthorization:\n  model: coarse permission strings, not machine-declared\n  strings: [orders:read, orders:write, webhooks:read, webhooks:write]\n  declared_in: operation descriptions only\n  contradiction: >-\n    /.well-known/api-onboarding.json states\
  \ \"There is no scope-string model. Access is gated by\n    plan tier.\" The OpenAPI names four permission strings across nine operations. The two provider\n    documents disagree, and no securityScheme exposes a scopes map either way -- so a caller\n    cannot discover what its key is permitted to do until a call fails.\n  plan_gate: >-\n    Feature access really is tiered on top of this: the Order API and partner webhooks unlock at\n    the $149/mo Pro Office plan.\nfailure_modes:\n  '401': >-\n    'A valid partner API key is required.' -- returned identically for a missing, malformed,\n    revoked or unknown key. Deliberately indistinguishable.\n  '403': >-\n    Reserved for a valid dashboard session that has not yet been linked to a partner. Before\n    2026-08-01, GET /api/partner/me also returned 403 for a missing credential; it now correctly\n    returns 401.\ntransport:\n  tls: TLSv1.3 observed on both hosts\n  hsts: true, max-age 63072000\n  see: security/signsealship-domain-security.yml\n\
  gaps:\n- No OAuth 2.0, no OIDC, no dynamic client registration (RFC 7591).\n- No self-serve API-key rotation.\n- No machine-readable scope or permission discovery.\n- Key delivery is out-of-band by email, which blocks fully programmatic onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/authentication/signsealship-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- notarization
- remote online notarization
- electronic signature
- document verification
- legal technology
- real estate
- title and escrow
- shipping
---
