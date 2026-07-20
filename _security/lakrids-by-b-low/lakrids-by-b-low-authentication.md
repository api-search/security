---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Lakrids By B Low Authentication
name_suffix: Authentication
oauth_flows: []
overview: LAKRIDS BY BÜLOW secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LAKRIDS BY BÜLOW
provider_slug: lakrids-by-b-low
scheme_count: 2
schemes:
- description: The BigCommerce Storefront GraphQL API requires a storefront API token sent as a bearer credential. Probed unauthenticated and rejected.
  docs: https://developer.bigcommerce.com/docs/storefront/graphql
  endpoint: https://lakridsbybulow.com/graphql
  evidence:
  - body: 'errors[0].message: "GraphQL credentials were missing. No token was sent."'
    method: POST
    status: 401
    url: https://lakridsbybulow.com/graphql
  - method: GET
    status: 405
    url: https://lakridsbybulow.com/graphql
  name: storefrontToken
  scheme: bearer
  type: http
- cookie_names:
  - SHOP_SESSION_TOKEN
  - SF-CSRF-TOKEN
  description: The BigCommerce Storefront REST API is session-scoped to the shopper's browser session; it returned 200 to an unauthenticated probe with an empty cart collection rather than an auth challenge.
  docs: https://developer.bigcommerce.com/docs/rest-storefront
  endpoint: https://lakridsbybulow.com/api/storefront
  evidence:
  - body: '[]'
    method: GET
    status: 200
    url: https://lakridsbybulow.com/api/storefront/carts
  in: cookie
  name: sessionCookie
  type: apiKey
slug: lakrids-by-b-low-authentication
source_filename: lakrids-by-b-low-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live HTTP probes of https://lakridsbybulow.com\ndocs: https://developer.bigcommerce.com/docs/storefront/graphql\nx-platform-provided: true\nx-platform: bigcommerce-stencil\nnotes: >-\n  LAKRIDS BY BÜLOW publishes no developer program and no first-party API\n  documentation. The auth model below belongs to the BigCommerce Stencil\n  storefront platform the brand runs on, observed live on the brand's own host.\n  It is recorded as probed evidence, not as a vendor claim by LAKRIDS BY BÜLOW.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: storefrontToken\n  type: http\n  scheme: bearer\n  endpoint: https://lakridsbybulow.com/graphql\n  description: >-\n    The BigCommerce Storefront GraphQL API requires a storefront API token sent\n    as a bearer credential. Probed unauthenticated and rejected.\n  evidence:\n  - method: POST\n    url: https://lakridsbybulow.com/graphql\n    status: 401\n  \
  \  body: 'errors[0].message: \"GraphQL credentials were missing. No token was sent.\"'\n  - method: GET\n    url: https://lakridsbybulow.com/graphql\n    status: 405\n  docs: https://developer.bigcommerce.com/docs/storefront/graphql\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  cookie_names:\n  - SHOP_SESSION_TOKEN\n  - SF-CSRF-TOKEN\n  endpoint: https://lakridsbybulow.com/api/storefront\n  description: >-\n    The BigCommerce Storefront REST API is session-scoped to the shopper's\n    browser session; it returned 200 to an unauthenticated probe with an empty\n    cart collection rather than an auth challenge.\n  evidence:\n  - method: GET\n    url: https://lakridsbybulow.com/api/storefront/carts\n    status: 200\n    body: '[]'\n  docs: https://developer.bigcommerce.com/docs/rest-storefront\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakrids-by-b-low/refs/heads/main/authentication/lakrids-by-b-low-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Consumer
- Consumer Goods
- Food and Beverage
- Confectionery
- Retail
- E-Commerce
- Denmark
---
