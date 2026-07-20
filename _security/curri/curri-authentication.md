---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Curri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curri secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Curri
provider_slug: curri
scheme_count: 1
schemes:
- description: 'Curri authenticates GraphQL requests with HTTP Basic authentication. The Authorization header carries a base64 encoding of your User ID and API key ("Authorization: Basic <base64(userId:apiKey)>"). Both a live API key and a separate Sandbox key are issued on account approval; the Sandbox key runs test deliveries with no drivers assigned and no charges processed.'
  name: BasicAuth
  scheme: basic
  sources:
  - https://docs.curri.com/docs/getting-started/tutorial
  type: http
slug: curri-authentication
source_filename: curri-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.curri.com/docs/getting-started/tutorial\ndocs: https://docs.curri.com/docs/getting-started\nsummary:\n  types: [http]\n  http_scheme: basic\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Curri authenticates GraphQL requests with HTTP Basic authentication. The\n      Authorization header carries a base64 encoding of your User ID and API\n      key (\"Authorization: Basic <base64(userId:apiKey)>\"). Both a live API key\n      and a separate Sandbox key are issued on account approval; the Sandbox key\n      runs test deliveries with no drivers assigned and no charges processed.\n    sources: [https://docs.curri.com/docs/getting-started/tutorial]\nendpoint: https://api.curri.com/graphql\nnotes: >-\n  Single GraphQL endpoint. No OAuth 2.0 / OpenID Connect surface is published,\n  so there is no scopes/ artifact for this provider; the\
  \ key + basic-auth model\n  is the complete authentication contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curri/refs/heads/main/authentication/curri-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Vertical Software
- Delivery
- Logistics
- Last Mile
- Freight
- Construction
- Supply Chain
- GraphQL
---
