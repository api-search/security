---
api_key_in:
- header
api_specs:
- filename: refurbed-buybackbidservice-api-openapi.yml
  format: yaml
  label: Refurbed BuybackBidService API
  slug: refurbed-buybackbidservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-buybackbidservice-api-openapi.yml
- filename: refurbed-buybackorderitemservice-api-openapi.yml
  format: yaml
  label: Refurbed BuybackOrderItemService API
  slug: refurbed-buybackorderitemservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-buybackorderitemservice-api-openapi.yml
- filename: refurbed-buybackorderservice-api-openapi.yml
  format: yaml
  label: Refurbed BuybackOrderService API
  slug: refurbed-buybackorderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-buybackorderservice-api-openapi.yml
- filename: refurbed-buybackproductservice-api-openapi.yml
  format: yaml
  label: Refurbed BuybackProductService API
  slug: refurbed-buybackproductservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-buybackproductservice-api-openapi.yml
- filename: refurbed-buybacksupplyboxservice-api-openapi.yml
  format: yaml
  label: Refurbed BuybackSupplyboxService API
  slug: refurbed-buybacksupplyboxservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-buybacksupplyboxservice-api-openapi.yml
- filename: refurbed-catalogservice-api-openapi.yml
  format: yaml
  label: Refurbed CatalogService API
  slug: refurbed-catalogservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-catalogservice-api-openapi.yml
- filename: refurbed-currencyservice-api-openapi.yml
  format: yaml
  label: Refurbed CurrencyService API
  slug: refurbed-currencyservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-currencyservice-api-openapi.yml
- filename: refurbed-instanceservice-api-openapi.yml
  format: yaml
  label: Refurbed InstanceService API
  slug: refurbed-instanceservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-instanceservice-api-openapi.yml
- filename: refurbed-marketofferservice-api-openapi.yml
  format: yaml
  label: Refurbed MarketOfferService API
  slug: refurbed-marketofferservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-marketofferservice-api-openapi.yml
- filename: refurbed-marketservice-api-openapi.yml
  format: yaml
  label: Refurbed MarketService API
  slug: refurbed-marketservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-marketservice-api-openapi.yml
- filename: refurbed-merchantservice-api-openapi.yml
  format: yaml
  label: Refurbed MerchantService API
  slug: refurbed-merchantservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-merchantservice-api-openapi.yml
- filename: refurbed-offerservice-api-openapi.yml
  format: yaml
  label: Refurbed OfferService API
  slug: refurbed-offerservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-offerservice-api-openapi.yml
- filename: refurbed-orderitemreturnservice-api-openapi.yml
  format: yaml
  label: Refurbed OrderItemReturnService API
  slug: refurbed-orderitemreturnservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-orderitemreturnservice-api-openapi.yml
- filename: refurbed-orderitemservice-api-openapi.yml
  format: yaml
  label: Refurbed OrderItemService API
  slug: refurbed-orderitemservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-orderitemservice-api-openapi.yml
- filename: refurbed-orderservice-api-openapi.yml
  format: yaml
  label: Refurbed OrderService API
  slug: refurbed-orderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-orderservice-api-openapi.yml
- filename: refurbed-productservice-api-openapi.yml
  format: yaml
  label: Refurbed ProductService API
  slug: refurbed-productservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-productservice-api-openapi.yml
- filename: refurbed-shippingprofileservice-api-openapi.yml
  format: yaml
  label: Refurbed ShippingProfileService API
  slug: refurbed-shippingprofileservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-shippingprofileservice-api-openapi.yml
- filename: refurbed-ticketservice-api-openapi.yml
  format: yaml
  label: Refurbed TicketService API
  slug: refurbed-ticketservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-ticketservice-api-openapi.yml
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
- Affiliates
- gRPC
---
