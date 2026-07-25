---
api_key_in: []
auth_types:
- oauth2
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Goldman Sachs Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Goldman Sachs secures its APIs with oauth2, http, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Goldman Sachs
provider_slug: goldman-sachs
scheme_count: 4
schemes:
- applies_to:
  - Goldman Sachs Content Services API
  - Goldman Sachs Pricing & Risk Services API
  - Goldman Sachs Hedging Services API
  - Goldman Sachs Index Services API
  - Goldman Sachs Portfolio Services API
  - Goldman Sachs Data Services API
  - GS Quant Python Toolkit
  description: Marquee platform APIs (Content, Pricing & Risk, Hedging, Index, Portfolio, Data Services, and the GS Quant toolkit) authenticate a session with OAuth 2.0 application credentials (client_id / client_secret) issued to approved institutional clients, exchanged for a bearer token against the Marquee auth endpoint. GS Quant's GsSession wraps this flow (client_credentials or a Marquee cookie session).
  docs: https://developer.gs.com/docs/gsquant/authentication/gs-session/
  flow: clientCredentials
  name: MarqueeOAuth2
  type: oauth2
- applies_to:
  - Goldman Sachs Transaction Banking (TxB) API
  description: Transaction Banking (TxB) requires a mutual-TLS connection (client certificate) plus IP allowlisting as the transport-layer trust anchor.
  docs: https://developer.gs.com/docs/services/transaction-banking/auth-connection/
  name: TxBmTLS
  type: mutualTLS
- applies_to:
  - Goldman Sachs Transaction Banking (TxB) API
  bearerFormat: JWT
  description: On top of mTLS, each TxB call carries an RSA-signed JWT in the request Authentication parameter. The JWT payload binds the caller identity (subject = client, issuer = partner, audience = txb), the signing key id (kid), and a SHA-256 hash of the presented mTLS certificate. Sensitive operations (e.g. acting on a third-party account) require an additional per-call step-up JWT.
  docs: https://developer.gs.com/docs/services/transaction-banking/auth-connection-part2
  name: TxBJWTStepUp
  scheme: bearer
  type: http
- applies_to:
  - Goldman Sachs RIA Custody API
  description: GS Custody Solutions (RIA Custody) REST APIs authenticate with OAuth 2.0 using a clientId and clientSecret issued by GSCS after partner approval (credentials delivered via Lockbox or secure email).
  docs: https://developer.gs.com/docs/services/ria-custody/authentication/
  flow: clientCredentials
  name: RIACustodyOAuth2
  type: oauth2
slug: goldman-sachs-authentication
source_filename: goldman-sachs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  https://developer.gs.com/docs/gsquant/authentication/gs-session/,\n  https://developer.gs.com/docs/services/transaction-banking/auth-connection/,\n  https://developer.gs.com/docs/services/transaction-banking/auth-connection-part2,\n  https://developer.gs.com/docs/services/ria-custody/authentication/\nnotes: >-\n  Goldman Sachs' three public developer surfaces use three distinct auth models.\n  Derived from the published authentication docs (the specs themselves are gated;\n  developer.gs.com blocks automated fetch, so schemes are captured from the docs\n  and search results rather than an OpenAPI securitySchemes block).\nsummary:\n  types: [oauth2, http, mutualTLS]\n  oauth2_flows: [clientCredentials]\n  surfaces: 3\nschemes:\n  - name: MarqueeOAuth2\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      Marquee platform APIs (Content, Pricing & Risk, Hedging, Index, Portfolio,\n      Data Services,\
  \ and the GS Quant toolkit) authenticate a session with OAuth\n      2.0 application credentials (client_id / client_secret) issued to approved\n      institutional clients, exchanged for a bearer token against the Marquee\n      auth endpoint. GS Quant's GsSession wraps this flow (client_credentials or\n      a Marquee cookie session).\n    applies_to:\n      - Goldman Sachs Content Services API\n      - Goldman Sachs Pricing & Risk Services API\n      - Goldman Sachs Hedging Services API\n      - Goldman Sachs Index Services API\n      - Goldman Sachs Portfolio Services API\n      - Goldman Sachs Data Services API\n      - GS Quant Python Toolkit\n    docs: https://developer.gs.com/docs/gsquant/authentication/gs-session/\n  - name: TxBmTLS\n    type: mutualTLS\n    description: >-\n      Transaction Banking (TxB) requires a mutual-TLS connection (client\n      certificate) plus IP allowlisting as the transport-layer trust anchor.\n    applies_to:\n      - Goldman Sachs Transaction Banking\
  \ (TxB) API\n    docs: https://developer.gs.com/docs/services/transaction-banking/auth-connection/\n  - name: TxBJWTStepUp\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      On top of mTLS, each TxB call carries an RSA-signed JWT in the request\n      Authentication parameter. The JWT payload binds the caller identity\n      (subject = client, issuer = partner, audience = txb), the signing key id\n      (kid), and a SHA-256 hash of the presented mTLS certificate. Sensitive\n      operations (e.g. acting on a third-party account) require an additional\n      per-call step-up JWT.\n    applies_to:\n      - Goldman Sachs Transaction Banking (TxB) API\n    docs: https://developer.gs.com/docs/services/transaction-banking/auth-connection-part2\n  - name: RIACustodyOAuth2\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      GS Custody Solutions (RIA Custody) REST APIs authenticate with OAuth 2.0\n      using a clientId and clientSecret\
  \ issued by GSCS after partner approval\n      (credentials delivered via Lockbox or secure email).\n    applies_to:\n      - Goldman Sachs RIA Custody API\n    docs: https://developer.gs.com/docs/services/ria-custody/authentication/\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goldman-sachs/refs/heads/main/authentication/goldman-sachs-authentication.yml
summary_line: oauth2/http/mutualTLS · 4 schemes
tags:
- Banking
- Financial
- Investment Banking
- Money Center
- Institutional
- Transaction Banking
- Custody
- Market Data
- United States
- Fortune 100
---
