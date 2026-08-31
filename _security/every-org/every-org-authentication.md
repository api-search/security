---
api_key_in: []
auth_types: []
description: Every.org's Partner (Charity) API authenticates with two classes of API key issued from the Every.org developer dashboard. Public keys authorize read access to publicly available nonprofit data and are passed as a URL query parameter; private keys authorize privileged account actions and are presented over HTTP Basic authentication with a public key as the username. There is no OAuth 2.0, OpenID Connect, or mutual-TLS surface — no /.well-known/oauth-authorization-server or /.well-known/openid-configuration document is served on any Every.org host (all probed 404 on 2026-08-28).
kind: authentication
layout: security
method: searched
name: Every Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Every.org declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Every.org
provider_slug: every-org
scheme_count: 2
schemes:
- applies_to:
  - GET /v0.2/nonprofit/{identifier}
  - GET /v0.2/search/{searchTerm}
  - GET /v0.2/browse/{cause}
  - GET /v0.2/nonprofit/{nonprofitIdentifier}/fundraiser/{fundraiserIdentifier}
  - GET /v0.2/nonprofit/{nonprofitIdentifier}/fundraiser/{fundraiserIdentifier}/raised
  description: Required to query publicly accessible data. Endpoints that accept only public-key authentication accept GET requests only. Public keys are explicitly documented as safe for both server-side and public-facing client-side use, though Every.org reserves the right to block a key for inappropriate usage.
  example: https://partners.every.org/v0.2/search/pets?apiKey=REDACTED_PUBLIC_KEY
  id: publicKeyQuery
  in: query
  label: Public key
  name: apiKey
  secret: false
  type: apiKey
- applies_to:
  - POST /v0.2/fundraiser
  description: Required for privileged, account-scoped writes. Username is any public key associated with the account; password is a private key associated with the same account. Documented as "must be kept out of publicly-accessible areas like client-side applications or version control".
  id: privateKeyBasic
  label: Private key
  password: private key
  scheme: basic
  secret: true
  type: http
  username: public key
slug: every-org-authentication
source_filename: every-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://docs.every.org/docs/endpoints/authentication\nprovider: Every.org\nproviderId: every-org\ndocs: https://docs.every.org/docs/endpoints/authentication\ndescription: >-\n  Every.org's Partner (Charity) API authenticates with two classes of API key issued from the\n  Every.org developer dashboard. Public keys authorize read access to publicly available nonprofit\n  data and are passed as a URL query parameter; private keys authorize privileged account actions\n  and are presented over HTTP Basic authentication with a public key as the username. There is no\n  OAuth 2.0, OpenID Connect, or mutual-TLS surface — no /.well-known/oauth-authorization-server or\n  /.well-known/openid-configuration document is served on any Every.org host (all probed 404 on\n  2026-08-28).\nkey_issuance:\n  console: https://www.every.org/charity-api\n  note: >-\n    Keys are generated from the developer dashboard after creating an Every.org account\
  \ at\n    every.org/charity-api. Private keys are shown ONCE at generation and are not retrievable\n    afterwards.\nschemes:\n  - id: publicKeyQuery\n    type: apiKey\n    in: query\n    name: apiKey\n    label: Public key\n    description: >-\n      Required to query publicly accessible data. Endpoints that accept only public-key\n      authentication accept GET requests only. Public keys are explicitly documented as safe for\n      both server-side and public-facing client-side use, though Every.org reserves the right to\n      block a key for inappropriate usage.\n    secret: false\n    applies_to:\n      - GET /v0.2/nonprofit/{identifier}\n      - GET /v0.2/search/{searchTerm}\n      - GET /v0.2/browse/{cause}\n      - GET /v0.2/nonprofit/{nonprofitIdentifier}/fundraiser/{fundraiserIdentifier}\n      - GET /v0.2/nonprofit/{nonprofitIdentifier}/fundraiser/{fundraiserIdentifier}/raised\n    example: https://partners.every.org/v0.2/search/pets?apiKey=REDACTED_PUBLIC_KEY\n  - id: privateKeyBasic\n\
  \    type: http\n    scheme: basic\n    label: Private key\n    description: >-\n      Required for privileged, account-scoped writes. Username is any public key associated with\n      the account; password is a private key associated with the same account. Documented as\n      \"must be kept out of publicly-accessible areas like client-side applications or version\n      control\".\n    secret: true\n    username: public key\n    password: private key\n    applies_to:\n      - POST /v0.2/fundraiser\ntransport:\n  https_required: true\n  hsts: max-age=15552000; includeSubDomains; preload\nmissing_on_401:\n  observed: >-\n    An unauthenticated GET https://partners.every.org/v0.2/search/pets returns HTTP 400 with the\n    plain-text body \"API key missing\" — not 401, and not a structured error object.\n  probed: '2026-08-28'\noauth: false\noidc: false\nmtls: false\nscopes:\n  supported: false\n  note: >-\n    Key-auth only. There is no scope or permission surface to enumerate, so no scopes/\
  \ artifact\n    is emitted (per the pipeline's OAuth-only rule for scopes).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/every-org/refs/heads/main/authentication/every-org-authentication.yml
summary_line: 2 schemes
tags:
- Charities
- Donations
- Fundraising
- Nonprofits
- Philanthropy
- Webhooks
- Giving
---
