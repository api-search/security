---
api_key_in:
- header
api_specs:
- filename: refurbed-merchant-api-openapi.json
  format: json
  label: Refurbed Merchant API
  slug: refurbed-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-merchant-api-openapi.json
- filename: refurbed-affiliate-api-openapi.json
  format: json
  label: Refurbed Affiliate Partner API
  slug: refurbed-affiliate-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-affiliate-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Refurbed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Refurbed secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Refurbed
provider_slug: refurbed
scheme_count: 1
schemes:
- description: 'Secret token passed in the Authorization header using the "Plain" method (e.g. "Authorization: Plain <token>"). The identical token is used as gRPC call metadata. Credentials are provisioned manually by refurbed.'
  in: header
  name: APIKeyAuth
  parameter: Authorization
  scheme_prefix: Plain
  sources:
  - openapi/refurbed-affiliate-api-openapi.json
  - openapi/refurbed-merchant-api-openapi.json
  type: apiKey
slug: refurbed-authentication
source_filename: refurbed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/refurbed-affiliate-api-openapi.json, openapi/refurbed-merchant-api-openapi.json\ndocs: https://gitlab.com/refurbed-community/public-apis/-/blob/master/refurbed_merchant_api/refb/merchant/v1/README.md\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  # Same secret token authenticates both the HTTP/JSON and the gRPC transport.\n  # Tokens are issued by refurbed (contact your account/partnership manager);\n  # there is no self-service OAuth or key-rotation portal documented.\n  token_scheme: Plain\n  header_example: 'Authorization: Plain f4e133d1-6cc4-4792-be5d-80a446a3d0dd'\n  grpc_metadata: authorization = \"Plain <token>\"\n  issuance: manual (account manager / integrations@refurbed.com)\nschemes:\n- name: APIKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_prefix: Plain\n  description: >-\n    Secret token passed in the Authorization header using the \"Plain\" method\n    (e.g.\
  \ \"Authorization: Plain <token>\"). The identical token is used as gRPC\n    call metadata. Credentials are provisioned manually by refurbed.\n  sources:\n  - openapi/refurbed-affiliate-api-openapi.json\n  - openapi/refurbed-merchant-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/authentication/refurbed-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketplace
- E-Commerce
- Refurbished Electronics
- Sustainability
- Circular Economy
- Retail
- Merchant API
- Affiliate
- gRPC
---
