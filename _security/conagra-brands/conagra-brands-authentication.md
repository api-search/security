---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Conagra Brands Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conagra Brands declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Conagra Brands
provider_slug: conagra-brands
scheme_count: 1
schemes:
- applies_to: every entity set that resolves (Products, Brands)
  description: No credential of any kind is required or accepted. Plain HTTPS GET with no Authorization header, no API key parameter and no cookie returned 200 on /odata, /odata/Products and /odata/Brands.
  evidence:
  - status: 200
    url: https://brands-api.conagrafoods.com/odata/Products?$top=1
  - status: 200
    url: https://brands-api.conagrafoods.com/odata/Brands('WES')
  id: none
  type: none
slug: conagra-brands-authentication
source_filename: conagra-brands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  Live anonymous requests to https://brands-api.conagrafoods.com/odata on 2026-09-05.\n  There is no published auth documentation to search - Conagra ships no developer portal.\nnote: >-\n  Derived by observation, not from a securityScheme block: this provider publishes no\n  OpenAPI, so derive-authentication.py had nothing to read. Everything below is what the\n  running service did in response to an unauthenticated request.\napi: Conagra Brand Sites API\nbase_url: https://brands-api.conagrafoods.com/odata\nschemes:\n  - id: none\n    type: none\n    description: >-\n      No credential of any kind is required or accepted. Plain HTTPS GET with no\n      Authorization header, no API key parameter and no cookie returned 200 on\n      /odata, /odata/Products and /odata/Brands.\n    evidence:\n      - url: https://brands-api.conagrafoods.com/odata/Products?$top=1\n        status: 200\n      - url: https://brands-api.conagrafoods.com/odata/Brands('WES')\n\
  \        status: 200\n    applies_to: every entity set that resolves (Products, Brands)\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  www_authenticate_challenge: none observed\ntransport:\n  https: true\n  http_redirects_to_https: false\n  note: >-\n    http://brands-api.conagrafoods.com/odata/$metadata answered over plain HTTP without\n    a redirect to HTTPS; HTTPS is available and is the URL the service document\n    self-declares (xml:base https://brands-api.conagrafoods.com/odata).\ncors:\n  access_control_allow_origin: '*'\n  access_control_allow_headers: Content-Type\n  note: >-\n    The wildcard CORS policy means any web page can call this API directly from a\n    browser. Combined with the absence of authentication, the entire product catalogue\n    is public read data.\nobservations:\n  - >-\n    Anonymous public read is almost certainly intentional - this service backs Conagra's\n    consumer brand websites, which\
  \ are public - but it is undocumented, so a consumer has\n    no stated terms, no rate limit and no support path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conagra-brands/refs/heads/main/authentication/conagra-brands-authentication.yml
summary_line: 1 scheme
tags:
- Branded Foods
- CPG
- Consumer Packaged Goods
- Food Service
- Fortune 500
- Frozen Foods
- Grocery
- OData
- Product Data
---
