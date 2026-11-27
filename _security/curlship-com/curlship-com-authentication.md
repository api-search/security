---
anonymous_access: true
api_key_in: []
api_specs:
- filename: curlship-com-badge-api-openapi.yml
  format: yaml
  label: CurlShip Badge API
  slug: curlship-com-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-badge-api-openapi.yml
- filename: curlship-com-billing-api-openapi.yml
  format: yaml
  label: CurlShip Billing API
  slug: curlship-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-billing-api-openapi.yml
- filename: curlship-com-edits-api-openapi.yml
  format: yaml
  label: CurlShip Edits API
  slug: curlship-com-edits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-edits-api-openapi.yml
- filename: curlship-com-listings-api-openapi.yml
  format: yaml
  label: CurlShip Listings API
  slug: curlship-com-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-listings-api-openapi.yml
- filename: curlship-com-stats-api-openapi.yml
  format: yaml
  label: CurlShip Stats API
  slug: curlship-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-stats-api-openapi.yml
- filename: curlship-com-x402-api-openapi.yml
  format: yaml
  label: CurlShip X402 API
  slug: curlship-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curlship-com/openapi/curlship-com-x402-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CurlShip Authentication
name_suffix: Authentication
oauth_flows: []
overview: CurlShip declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CurlShip
provider_slug: curlship-com
scheme_count: 3
schemes:
- description: No API key, account or login. Rate limits are applied per IP (and per listing for edits).
  source: https://curlship.com/llms.txt
  type: none
- declared_in_spec: false
  description: base64 JSON x402 v2 PaymentPayload -- the client's EIP-3009 TransferWithAuthorization signature, echoing the quote as `accepted`. Without it the endpoint answers 402 with a PAYMENT-REQUIRED quote.
  in: header
  name: PAYMENT-SIGNATURE
  note: Declared in the spec as a header parameter on these two operations, not as a securityScheme.
  operations:
  - x402Submit
  - x402Feature
  role: payment-authorization (x402 v2), not identity
  type: apiKey
- description: createEditRequest takes proof "email" (a one-time confirmation link mailed to the registered address) or proof "domain" (a token published at /.well-known/curlship-verify.txt or a <meta name="curlship-verify"> tag on BOTH the listed and new site), confirmed via confirmEditRequest.
  operations:
  - createEditRequest
  - confirmEditRequest
  - getEditRequest
  source: https://curlship.com/llms.txt
  type: ownership-proof
slug: curlship-com-authentication
source_filename: curlship-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://curlship.com/openapi.json\n- https://curlship.com/llms.txt\ndocs: https://curlship.com/docs\nsummary: The OpenAPI declares no securitySchemes. The docs state \"No CAPTCHA, no login, no approval queue\" -- every endpoint is called anonymously. Payment on the x402 endpoints is carried by a signed PAYMENT-SIGNATURE header, and edits to an existing listing are authorized by an ownership proof (email confirmation link or a domain token), not by credentials.\nschemes:\n- type: none\n  description: No API key, account or login. Rate limits are applied per IP (and per listing for edits).\n  source: https://curlship.com/llms.txt\n- type: apiKey\n  in: header\n  name: PAYMENT-SIGNATURE\n  role: payment-authorization (x402 v2), not identity\n  description: base64 JSON x402 v2 PaymentPayload -- the client's EIP-3009 TransferWithAuthorization signature, echoing the quote as `accepted`. Without it the endpoint answers 402 with\
  \ a PAYMENT-REQUIRED quote.\n  operations: [x402Submit, x402Feature]\n  declared_in_spec: false\n  note: Declared in the spec as a header parameter on these two operations, not as a securityScheme.\n- type: ownership-proof\n  description: 'createEditRequest takes proof \"email\" (a one-time confirmation link mailed to the registered address) or proof \"domain\" (a token published at /.well-known/curlship-verify.txt or a <meta name=\"curlship-verify\"> tag on BOTH the listed and new site), confirmed via confirmEditRequest.'\n  operations: [createEditRequest, confirmEditRequest, getEditRequest]\n  source: https://curlship.com/llms.txt\n"
source_yaml_url: https://artifacts.apis.io/curlship-com/authentication/curlship-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Directory
- Product Listings
- Developer Tools
- MCP
- AI Agents
- REST API
- Launch Platform
---
