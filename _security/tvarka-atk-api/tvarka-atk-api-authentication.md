---
api_key_in:
- query
api_specs:
- filename: tvarka-atk-api-auth-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Auth API
  slug: tvarka-atk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-auth-api-openapi.yml
- filename: tvarka-atk-api-erasure-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Erasure API
  slug: tvarka-atk-api-erasure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-erasure-api-openapi.yml
- filename: tvarka-atk-api-ltv-api-openapi.yml
  format: yaml
  label: Tvarka ATK API LTV API
  slug: tvarka-atk-api-ltv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-ltv-api-openapi.yml
- filename: tvarka-atk-api-pairing-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Pairing API
  slug: tvarka-atk-api-pairing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-pairing-api-openapi.yml
- filename: tvarka-atk-api-sign-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Sign API
  slug: tvarka-atk-api-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-sign-api-openapi.yml
- filename: tvarka-atk-api-tvarka-atk-api-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Tvarka ATK API API
  slug: tvarka-atk-api-tvarka-atk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-tvarka-atk-api-api-openapi.yml
- filename: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Tvarka ATK QES Signing API (paid Tier Addendum) API
  slug: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api-openapi.yml
- filename: tvarka-atk-api-validation-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Validation API
  slug: tvarka-atk-api-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-validation-api-openapi.yml
- filename: tvarka-atk-api-well-known-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Well Known API
  slug: tvarka-atk-api-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-well-known-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tvarka Atk Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tvarka ATK API secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tvarka ATK API
provider_slug: tvarka-atk-api
scheme_count: 3
schemes:
- description: 'Provider server-to-server credentials `keyId:keySecret`. Server-to-server only, also gated by the

    provider''s server IP allow-list. Never placed in a browser/mobile client.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tvarka-atk-api-auth-openapi.yaml
  - openapi/tvarka-atk-api-openapi-original.json
  - openapi/tvarka-atk-api-sign-openapi.yaml
  type: http
- bearerFormat: JWT
  description: 'Short-lived, per-request JWT (`ES256`) minted at request creation, scoped

    `{tenant, requestId, purpose, method, allowedOrigins}`. Safe to hand to a browser/mobile client:

    it cannot create requests, read tenant data, or touch other requests. For browser clients the API

    enforces `Origin` against `allowedOrigins` (rejects cross-origin replay).'
  name: clientToken
  scheme: bearer
  sources:
  - openapi/tvarka-atk-api-auth-openapi.yaml
  - openapi/tvarka-atk-api-openapi-original.json
  - openapi/tvarka-atk-api-sign-openapi.yaml
  type: http
- description: One-off token returned with a completed sign result, for fetching the signed document.
  in: query
  name: downloadToken
  parameter: downloadToken
  sources:
  - openapi/tvarka-atk-api-openapi-original.json
  - openapi/tvarka-atk-api-sign-openapi.yaml
  type: apiKey
slug: tvarka-atk-api-authentication
source_filename: tvarka-atk-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://atk.tvarka.pro/docs/quickstart/ + openapi/tvarka-atk-api-openapi-original.json\nsummary:\n  types:\n  - http\n  - apiKey\n  http_schemes:\n  - basic\n  - bearer\n  api_key_in:\n  - query\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  model: layered - a long-lived provider secret on the backend, a short-lived request-scoped token on\n    the device\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Provider server-to-server credentials `keyId:keySecret`. Server-to-server only, also gated\n    by the\n\n    provider''s server IP allow-list. Never placed in a browser/mobile client.'\n  sources:\n  - openapi/tvarka-atk-api-auth-openapi.yaml\n  - openapi/tvarka-atk-api-openapi-original.json\n  - openapi/tvarka-atk-api-sign-openapi.yaml\n- name: clientToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Short-lived, per-request JWT (`ES256`) minted at request\
  \ creation, scoped\n\n    `{tenant, requestId, purpose, method, allowedOrigins}`. Safe to hand to a browser/mobile client:\n\n    it cannot create requests, read tenant data, or touch other requests. For browser clients the API\n\n    enforces `Origin` against `allowedOrigins` (rejects cross-origin replay).'\n  sources:\n  - openapi/tvarka-atk-api-auth-openapi.yaml\n  - openapi/tvarka-atk-api-openapi-original.json\n  - openapi/tvarka-atk-api-sign-openapi.yaml\n- name: downloadToken\n  type: apiKey\n  in: query\n  parameter: downloadToken\n  description: One-off token returned with a completed sign result, for fetching the signed document.\n  sources:\n  - openapi/tvarka-atk-api-openapi-original.json\n  - openapi/tvarka-atk-api-sign-openapi.yaml\ndocs: https://atk.tvarka.pro/docs/quickstart/\nmodel:\n  server_to_server: HTTP Basic keyId:keySecret, additionally gated by the provider server IP allow-list.\n    Document-level default security. Creates requests, polls, cancels, erases, downloads\
  \ and calls the\n    trust services. Never placed in a browser or mobile client.\n  client: A per-request ES256 JWT (clientToken) minted at request creation and scoped {tenant, requestId,\n    purpose, method, allowedOrigins}. It cannot create requests, read tenant data or touch another request.\n    For browser clients the API enforces Origin against allowedOrigins and rejects cross-origin replay.\n  download: A one-off downloadToken query parameter returned with a completed result.\n  operation_token: 'Not a securityScheme, but a second single-use factor inside the ceremony: the operationToken\n    returned with the data-to-be-signed must be presented on complete, and is spent on first use (409\n    operation_token_spent).'\n  unauthenticated: 'claimPairing (POST /pairing/claim) declares security: [] - possession of the short-lived\n    one-claim pairing token is the credential. getJwks is also public.'\ncredential_issuance:\n  url: https://atk.tvarka.pro/docs/access/\n  process: Manual\
  \ review; the credential-claim link is emailed but the secret itself is never emailed.\n  environments:\n  - sandbox\n  - production\n  note: The environment is a property of the issued credential, not a separate host or key prefix.\nfailure_codes:\n- invalid_basic_credentials (401)\n- invalid_client_token (401)\n- client_token_expired (401)\n- operation_token_expired (401)\n- invalid_download_token (401)\n- origin_not_allowed (403)\n- ip_not_allowed (403)\n- tenant_suspended (403)\n- tier_forbidden (403)\n- operation_token_spent (409)\nverification:\n  jwks: well-known/tvarka-atk-api-atk-jwks.json\n  note: The optional identity assertion JWT is verifiable against the published JWKS (kid atk-1, ES256).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/authentication/tvarka-atk-api-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Authentication
- Digital Signature
- eIDAS
- QES
- Lithuania
- OpenAPI
- eID
- Smart-ID
- Mobile-ID
- NFC
- Timestamping
- LTV
- Webhooks
- Identity
- Trust Services
- GDPR
---
