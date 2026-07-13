---
api_key_in:
- header
api_specs:
- filename: etsy-openapi-original.yml
  format: yaml
  label: Etsy Open API v3
  slug: open-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/openapi/etsy-openapi-original.yml
- filename: etsy-webhooks-asyncapi.yml
  format: yaml
  label: Etsy Open API v3 Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/asyncapi/etsy-webhooks-asyncapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Etsy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Etsy secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Etsy
provider_slug: etsy
scheme_count: 2
schemes:
- description: Every request to a v3 API endpoint must include this data in the format `keystring:shared_secret`. Your keystring and shared secret are available on the [Your Apps](https://www.etsy.com/developers/your-apps) page.
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/etsy-openapi-original.yml
  type: apiKey
- description: Open API v3 supports authenticating via OAuth 2.0. More information about Etsy's specific implementation of OAuth2 can be found [here](/documentation/essentials/oauth2).
  flows:
  - authorizationUrl: https://www.etsy.com/oauth/connect
    flow: authorizationCode
    scopes: 20
    tokenUrl: https://openapi.etsy.com/v3/public/oauth/token
  name: oauth2
  sources:
  - openapi/etsy-openapi-original.yml
  type: oauth2
slug: etsy-authentication
source_filename: etsy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/etsy-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Every request to a v3 API endpoint must include this data in the format `keystring:shared_secret`.\n    Your keystring and shared secret are available on the [Your Apps](https://www.etsy.com/developers/your-apps)\n    page.\n  sources:\n  - openapi/etsy-openapi-original.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.etsy.com/oauth/connect\n    tokenUrl: https://openapi.etsy.com/v3/public/oauth/token\n    scopes: 20\n  description: Open API v3 supports authenticating via OAuth 2.0. More information about Etsy's\n    specific implementation of OAuth2 can be found [here](/documentation/essentials/oauth2).\n  sources:\n  - openapi/etsy-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/authentication/etsy-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Marketplace
- Ecommerce
- Handmade
- Listings
- Orders
- Payments
- Reviews
- Shipping
- Taxonomy
- OAuth2
---
