---
api_key_in:
- header
api_specs:
- filename: shopmy-partners-openapi.yml
  format: yaml
  label: ShopMy Partners API
  slug: shopmy-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/openapi/shopmy-partners-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Shopmy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ShopMy secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ShopMy
provider_slug: shopmy
scheme_count: 3
schemes:
- description: 'Brand/developer key sent as `Authorization: Bearer <developer key>`. Found in Brand Account Settings under Tokens > Developer Key.'
  name: developerKey
  scheme: bearer
  sources:
  - openapi/shopmy-partners-openapi.yml
  type: http
- description: 'Per-user long-term OAuth access token sent as `X-ACCESS-TOKEN: Bearer <access token>`, obtained via the OAuth token exchange.'
  in: header
  name: accessToken
  parameter: X-ACCESS-TOKEN
  sources:
  - openapi/shopmy-partners-openapi.yml
  type: apiKey
- description: OAuth 2.0 authorization-code flow for acting on behalf of ShopMy users.
  flows:
  - authorizationUrl: https://shopmy.us/oauth
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://api.shopmy.us/v1/Partners/oauth-exchange-token
  name: oauth2
  sources:
  - openapi/shopmy-partners-openapi.yml
  type: oauth2
slug: shopmy-authentication
source_filename: shopmy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/shopmy-partners-openapi.yml\ndocs: https://docs.shopmy.us/reference/getting-started-with-your-api-1\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: developerKey\n  type: http\n  scheme: bearer\n  description: 'Brand/developer key sent as `Authorization: Bearer <developer key>`. Found in\n    Brand Account Settings under Tokens > Developer Key.'\n  sources:\n  - openapi/shopmy-partners-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: X-ACCESS-TOKEN\n  description: 'Per-user long-term OAuth access token sent as `X-ACCESS-TOKEN: Bearer <access\n    token>`, obtained via the OAuth token exchange.'\n  sources:\n  - openapi/shopmy-partners-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopmy.us/oauth\n    tokenUrl: https://api.shopmy.us/v1/Partners/oauth-exchange-token\n\
  \    scopes: 5\n  description: OAuth 2.0 authorization-code flow for acting on behalf of ShopMy users.\n  sources:\n  - openapi/shopmy-partners-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/authentication/shopmy-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Commerce
- Creator Economy
- Creator Commerce
- Affiliate Marketing
- Influencer Marketing
- E-Commerce
- Retail
---
