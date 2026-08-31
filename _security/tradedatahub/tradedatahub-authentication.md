---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: TradeDataHub Public API
  slug: tradedatahub-public-api
  spec_type: OpenAPI
  url: https://www.tradedatahub.net/openapi.json
auth_types: []
description: TradeDataHub publishes NO securitySchemes in its OpenAPI 3.1.0 contract, and none of the eleven documented operations declares a security requirement. Every discovery endpoint under /api/v1/ is genuinely unauthenticated and was called anonymously during this pass. The only credential-bearing surface is the paid retrieval endpoint, which uses an x402 PAYMENT-SIGNATURE header rather than an API key, bearer token or OAuth flow.
kind: authentication
layout: security
method: searched
name: Tradedatahub Authentication
name_suffix: Authentication
oauth_flows: []
overview: TradeDataHub Public API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: TradeDataHub Public API
provider_slug: tradedatahub
scheme_count: 0
schemes: []
slug: tradedatahub-authentication
source_filename: tradedatahub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://www.tradedatahub.net/developers/\nspec: openapi/tradedatahub-openapi.json\ndocs: https://www.tradedatahub.net/developers/\nname: TradeDataHub authentication profile\ndescription: >-\n  TradeDataHub publishes NO securitySchemes in its OpenAPI 3.1.0 contract, and none of the eleven\n  documented operations declares a security requirement. Every discovery endpoint under /api/v1/ is\n  genuinely unauthenticated and was called anonymously during this pass. The only credential-bearing\n  surface is the paid retrieval endpoint, which uses an x402 PAYMENT-SIGNATURE header rather than an\n  API key, bearer token or OAuth flow.\nschemes: []\nscheme_count: 0\nobserved:\n  - surface: Free discovery endpoints (/api/v1/coverage, /states, /trades, /cities, /datasets, /datasets/{product_id}, /price, /preview, /texas-trades-teaser.json)\n    model: none\n    credential: null\n    evidence:\n      url: https://www.tradedatahub.net/api/v1/coverage\n\
  \      http_status: 200\n      note: Returned live JSON with no Authorization header sent.\n  - surface: Paid retrieval (/api/v1/datasets/{product_id}/download)\n    model: x402-payment-header\n    credential: PAYMENT-SIGNATURE request header\n    declared_in_spec: false\n    network: Base Sepolia (eip155:84532) — TESTNET ONLY\n    evidence:\n      url: https://www.tradedatahub.net/api/v1/datasets/state:california/download\n      http_status: 402\n      note: >-\n        An unpaid GET returns HTTP 402 with a base64 Payment-Required header and a JSON\n        payment_required body carrying the x402 v2 challenge. Probed anonymously; no payment made.\ncors:\n  access_control_allow_origin: '*'\n  access_control_allow_methods: GET, HEAD, OPTIONS\n  access_control_allow_headers: Content-Type, Authorization, X-Requested-With, Payment-Signature\n  access_control_expose_headers: Payment-Required, Payment-Response\n  note: Observed on live responses from www.tradedatahub.net.\ngaps:\n  - >-\n  \
  \  The x402 PAYMENT-SIGNATURE requirement is documented in prose (llms-full.txt and /developers/)\n    but is NOT expressed as an OpenAPI securityScheme, so a generated client cannot discover it.\n    An apiKey-in-header scheme named PAYMENT-SIGNATURE applied to the download operation would close this.\n  - >-\n    Human purchasing runs through Stripe Checkout, and API access for higher-volume use is negotiated by\n    email (tradedatahub@gmail.com per /api/v1/texas-trades-teaser.json). There is no self-serve key issuance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradedatahub/refs/heads/main/authentication/tradedatahub-authentication.yml
summary_line: 0 schemes
tags:
- contractor data
- B2B data
- business listings
- datasets
- CSV
- lead generation
- sales intelligence
- x402
- agent-native
- llms.txt
- OpenAPI
---
