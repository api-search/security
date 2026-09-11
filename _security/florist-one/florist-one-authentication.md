---
anonymous_access: false
api_key_in: []
api_specs:
- filename: florist-one-affiliate-api-openapi.yml
  format: yaml
  label: Florist One Affiliate API
  slug: florist-one-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/florist-one/refs/heads/main/openapi/florist-one-affiliate-api-openapi.yml
- filename: florist-one-flowershop-api-openapi.yml
  format: yaml
  label: Florist One FlowerShop API
  slug: florist-one-flowershop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/florist-one/refs/heads/main/openapi/florist-one-flowershop-api-openapi.yml
- filename: florist-one-giftbaskets-api-openapi.yml
  format: yaml
  label: Florist One GiftBaskets API
  slug: florist-one-giftbaskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/florist-one/refs/heads/main/openapi/florist-one-giftbaskets-api-openapi.yml
- filename: florist-one-shoppingcart-api-openapi.yml
  format: yaml
  label: Florist One ShoppingCart API
  slug: florist-one-shoppingcart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/florist-one/refs/heads/main/openapi/florist-one-shoppingcart-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Florist One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Florist One secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Florist One
provider_slug: florist-one
scheme_count: 1
schemes:
- description: HTTP Basic auth with API Key as username and assigned password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/_original/florist-one-openapi.yml
  - openapi/florist-one-flowershop-api-openapi.yml
  - openapi/florist-one-giftbaskets-api-openapi.yml
  - openapi/florist-one-shoppingcart-api-openapi.yml
  - openapi/florist-one-affiliate-api-openapi.yml
  type: http
slug: florist-one-authentication
source_filename: florist-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: >-\n  https://www.floristone.com/api/technical-information/,\n  https://www.floristone.com/api/print_api_legal/,\n  https://github.com/fhwsolutions/FloristOne_API (Florist One's published sample code),\n  live probe of https://www.floristone.com/api/rest/flowershop/getproducts,\n  openapi/_original/florist-one-openapi.yml\ndocs: https://www.floristone.com/api/technical-information/\ndocs_note: >-\n  The auth documentation page is itself gated — https://www.floristone.com/api/technical-information/\n  returns 200 but renders a login form asking for an API Key and Password. The credential\n  model below was reconstructed from Florist One's own public sample code and one live\n  probe, not from a published auth reference.\nsummary:\n  types:\n    - http\n  api_key_in: []\n  oauth2_flows: []\n  credential_issuance: manual, after signup at https://www.floristone.com/api/api-signup/\nschemes:\n  - name: basicAuth\n    type: http\n\
  \    scheme: basic\n    description: HTTP Basic auth with API Key as username and assigned password\n    sources:\n      - openapi/_original/florist-one-openapi.yml\n      - openapi/florist-one-flowershop-api-openapi.yml\n      - openapi/florist-one-giftbaskets-api-openapi.yml\n      - openapi/florist-one-shoppingcart-api-openapi.yml\n      - openapi/florist-one-affiliate-api-openapi.yml\ncredential:\n  username: API Key (a numeric key issued by Florist One)\n  password: assigned password\n  issuance: >-\n    Issued on signup at https://www.floristone.com/api/api-signup/. Accepting the API\n    Agreement is a condition of use — \"By clicking the Accept button for this Agreement\n    and/or using an API key issued by Provider, you confirm your acceptance\".\n  rotation: not documented\n  revocation: >-\n    Florist One may suspend or terminate API access for material breach, illegal or\n    fraudulent activity, or termination of a subcontractor's services (API Agreement,\n    section 5.2.2).\
  \ No self-service key rotation or revocation is documented.\n  multi_key_requirement: >-\n    An integrator selling into both the United States and Canada must hold TWO API keys and\n    swap them by order destination, because orders to the US are charged in USD and orders\n    to Canada in CAD. Published in https://www.floristone.com/api/flowers-api-faq/.\nwire_format:\n  header: Authorization\n  observed_form: 'Authorization: <base64(apikey:password)>'\n  rfc7617_conformant: false\n  deviation_note: >-\n    Every published sample — php/flowershop/placeorder.php, php/shoppingcart/*.php,\n    php/affiliate/legalagreement.php and the ColdFusion equivalents — builds the header as\n    base64_encode(\"{$username}:{$password}\") and sends it with NO `Basic ` scheme prefix.\n    RFC 7617 requires the scheme token. Whether the server accepts the RFC form as well is\n    not documented anywhere public, so an integrator using a standard HTTP client's\n    basic-auth helper cannot tell from the\
  \ documentation whether it will work.\n  transport: HTTPS only\nunauthenticated_behavior:\n  fetched: '2026-09-10'\n  url: https://www.floristone.com/api/rest/flowershop/getproducts?category=fx&count=2&start=1\n  http_status: 403\n  content_type: text/html\n  body: >-\n    Stock Microsoft IIS error page reading \"403 - Forbidden: Access is denied.\"\n  note: >-\n    No WWW-Authenticate challenge is returned, which is a further deviation from HTTP Basic\n    — a client is given no machine-readable indication of which scheme or realm to use. The\n    error is untyped HTML. See errors/florist-one-problem-types.yml.\nnot_supported:\n  oauth2: true\n  openid_connect: true\n  api_key_header: true\n  mutual_tls: true\n  scopes: >-\n    No scope, permission, or role model exists. One credential grants the whole surface,\n    including order placement. There is no read-only key, which means an agent given a key\n    to browse products is also holding a key that can charge a card.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/florist-one/refs/heads/main/authentication/florist-one-authentication.yml
summary_line: http · 1 scheme
tags:
- Delivery
- E-Commerce
- Florists
- Flowers
- Gifts
---
