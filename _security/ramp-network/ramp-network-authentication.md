---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Ramp Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ramp Network declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Ramp Network
provider_slug: ramp-network
scheme_count: 3
schemes:
- applies_to:
  - GET /host-api/v3/assets
  - GET /host-api/v3/offramp/assets
  - POST /host-api/v3/onramp/quote/all
  - POST /host-api/v3/offramp/quote/all
  - Ramp Instant SDK / widget initialisation
  - Hosted widget URL (https://app.rampnetwork.com/?hostApiKey=...)
  contact: partner@ramp.network
  description: The integration (partner) key. Issued by Ramp Network on request — there is no self-service key issuance. On the assets endpoints it is optional and unlocks an `enabledFeatures` list plus partner-specific configuration; on the quote endpoints the docs present it as the required identifier. It is also the key that attributes purchases to a partner integration for revenue share. Because it travels in the QUERY STRING and is embedded in client-side widget initialisation, it is a partner identifier rather than a secret.
  id: hostApiKey
  in: query
  name: hostApiKey
  obtain: https://docs.rampnetwork.com/api-keys
  required: conditional
  type: apiKey
- applies_to:
  - GET /host-api/purchase/{id}
  - GET /host-api/offramp/sale/{id}
  description: A per-transaction capability token (`purchaseViewToken` / `saleViewToken`) delivered with the PURCHASE_CREATED / OFFRAMP_SALE_CREATED SDK event and the corresponding webhook. It is passed as the `secret` query parameter and scopes read access to exactly one transaction. This is an object-capability model, not an account credential — possession of the token is the authorisation.
  id: purchaseViewToken
  in: query
  name: secret
  required: true
  type: apiKey
- algorithm: ECDSA over secp256k1 with SHA-256, DER signature, base64 encoded
  canonicalisation: JSON request body serialised with fast-json-stable-stringify (object keys sorted alphabetically, no whitespace)
  description: Ramp Network signs every outbound webhook call so the integrator can verify authenticity. This is the only cryptographic authentication in the surface, and it authenticates RAMP TO THE INTEGRATOR, not the other way round.
  direction: inbound-to-integrator
  docs: https://docs.rampnetwork.com/webhooks
  header: X-Body-Signature
  id: webhook-signature
  key_distribution: public keys published verbatim in the webhook documentation (separate production and demo keys)
  type: signature
slug: ramp-network-authentication
source_filename: ramp-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.rampnetwork.com/api-keys\ndocs: https://docs.rampnetwork.com/api-keys\nsummary: >-\n  Ramp Network has no OAuth surface and no bearer-token API. The public Host API is\n  largely ANONYMOUS — assets, prices, currencies, payment methods and payout methods\n  are readable with no credential at all (verified live on 2026-08-26 against\n  https://api.rampnetwork.com/api/host-api/v3/currencies, HTTP 200). Three distinct\n  credential mechanisms exist on top of that, and they are not interchangeable.\nschemes:\n  - id: hostApiKey\n    type: apiKey\n    in: query\n    name: hostApiKey\n    required: conditional\n    applies_to:\n      - GET /host-api/v3/assets\n      - GET /host-api/v3/offramp/assets\n      - POST /host-api/v3/onramp/quote/all\n      - POST /host-api/v3/offramp/quote/all\n      - Ramp Instant SDK / widget initialisation\n      - Hosted widget URL (https://app.rampnetwork.com/?hostApiKey=...)\n    description:\
  \ >-\n      The integration (partner) key. Issued by Ramp Network on request — there is no\n      self-service key issuance. On the assets endpoints it is optional and unlocks\n      an `enabledFeatures` list plus partner-specific configuration; on the quote\n      endpoints the docs present it as the required identifier. It is also the key\n      that attributes purchases to a partner integration for revenue share. Because\n      it travels in the QUERY STRING and is embedded in client-side widget\n      initialisation, it is a partner identifier rather than a secret.\n    obtain: https://docs.rampnetwork.com/api-keys\n    contact: partner@ramp.network\n  - id: purchaseViewToken\n    type: apiKey\n    in: query\n    name: secret\n    required: true\n    applies_to:\n      - GET /host-api/purchase/{id}\n      - GET /host-api/offramp/sale/{id}\n    description: >-\n      A per-transaction capability token (`purchaseViewToken` / `saleViewToken`)\n      delivered with the PURCHASE_CREATED\
  \ / OFFRAMP_SALE_CREATED SDK event and the\n      corresponding webhook. It is passed as the `secret` query parameter and scopes\n      read access to exactly one transaction. This is an object-capability model,\n      not an account credential — possession of the token is the authorisation.\n  - id: webhook-signature\n    type: signature\n    direction: inbound-to-integrator\n    header: X-Body-Signature\n    algorithm: ECDSA over secp256k1 with SHA-256, DER signature, base64 encoded\n    canonicalisation: >-\n      JSON request body serialised with fast-json-stable-stringify (object keys\n      sorted alphabetically, no whitespace)\n    key_distribution: public keys published verbatim in the webhook documentation (separate production and demo keys)\n    description: >-\n      Ramp Network signs every outbound webhook call so the integrator can verify\n      authenticity. This is the only cryptographic authentication in the surface,\n      and it authenticates RAMP TO THE INTEGRATOR,\
  \ not the other way round.\n    docs: https://docs.rampnetwork.com/webhooks\noauth2: false\nopenid_connect: false\nmutual_tls: false\ngaps:\n  - >-\n    No OAuth 2.0, no OpenID Connect, no scope model — so scopes/ is intentionally\n    not emitted for this provider.\n  - >-\n    hostApiKey is transmitted as a URL query parameter and is present in\n    client-side widget configuration, so it will appear in browser history, proxy\n    logs and referrer headers. The docs do not describe rotation or revocation.\n  - >-\n    No published authentication error catalogue; failures surface through the\n    generic `{ code, statusCode }` error envelope.\nevidence:\n  - url: https://docs.rampnetwork.com/api-keys\n    status: 200\n  - url: https://docs.rampnetwork.com/webhooks\n    status: 200\n  - url: https://api.rampnetwork.com/api/host-api/v3/currencies\n    status: 200\n    detail: returned the full currency list with no credential supplied\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramp-network/refs/heads/main/authentication/ramp-network-authentication.yml
summary_line: 3 schemes
tags:
- Cryptocurrency
- Payments
- Fintech
- On-Ramp
- Off-Ramp
- Blockchain
- Web3
- Wallets
- Digital Assets
- Compliance
- Embedded Finance
---
