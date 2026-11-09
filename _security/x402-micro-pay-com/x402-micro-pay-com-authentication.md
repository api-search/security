---
anonymous_access: false
api_key_in: []
api_specs:
- filename: x402-micro-pay-com-openapi-generated.yml
  format: yaml
  label: x402-micro-pay-com API
  slug: x402-micro-pay-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/x402-micro-pay-com/openapi/_ae-authored/x402-micro-pay-com-openapi-generated.yml
auth_types: []
description: Authentication is performed via the x402 payment protocol. Calls are initially sent without authentication, receive a 402 response with a PAYMENT-REQUIRED header, then the client signs a USDC transfer and retries with a PAYMENT-SIGNATURE header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: X402 Micro Pay Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: x402-micro-pay-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: x402-micro-pay-com
provider_slug: x402-micro-pay-com
scheme_count: 1
schemes:
- evidence: '← 402 Payment Required + PAYMENT-REQUIRED header: base64 JSON {x402Version: 2, accepts: [{scheme: "exact", network: "eip155:8453", asset: USDC, amount: "5000", payTo}]'
  header: PAYMENT-SIGNATURE
  how_to_obtain: Send an unpaid request, receive a 402 with PAYMENT-REQUIRED, sign a USDC transfer to the payTo address, then retry the request with the PAYMENT-SIGNATURE header.
  location: header
  name: x402 payment
  type: other
slug: x402-micro-pay-com-authentication
source_filename: x402-micro-pay-com-authentication.yml
source_heading: Authentication Profile
source_url: https://grokzilla.shop/docs/token-count
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://grokzilla.shop/docs/token-count\nsources:\n- https://grokzilla.shop/docs/token-count\n- https://grokzilla.shop/docs/token-price\n- https://grokzilla.shop/docs/token-risk\n- https://x402-micro-pay.com/try/token-risk\ndescription: Authentication is performed via the x402 payment protocol. Calls are initially sent without authentication, receive a 402 response\n  with a PAYMENT-REQUIRED header, then the client signs a USDC transfer and retries with a PAYMENT-SIGNATURE header.\nschemes:\n- type: other\n  name: x402 payment\n  evidence: '← 402 Payment Required + PAYMENT-REQUIRED header: base64 JSON {x402Version: 2, accepts: [{scheme: \"exact\", network: \"eip155:8453\",\n    asset: USDC, amount: \"5000\", payTo}]'\n  location: header\n  header: PAYMENT-SIGNATURE\n  how_to_obtain: Send an unpaid request, receive a 402 with PAYMENT-REQUIRED, sign a USDC transfer to the payTo address,\
  \ then retry the request\n    with the PAYMENT-SIGNATURE header.\ndocs: https://grokzilla.shop/docs/token-count\n"
source_yaml_url: https://artifacts.apis.io/x402-micro-pay-com/authentication/x402-micro-pay-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Payments
- Microservices
- Marketplace
---
