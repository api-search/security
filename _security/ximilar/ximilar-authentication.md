---
api_key_in:
- header
auth_types:
- apiKey
description: Ximilar uses a single long-lived API token issued per account in the Ximilar App. There is no OAuth 2.0, no OpenID Connect, no mTLS and no scope system; every request on every service carries the same token. Derived from the provider's own Quickstart page, not from a specification — Ximilar publishes no OpenAPI, so there are no securitySchemes to aggregate.
kind: authentication
layout: security
method: searched
name: Ximilar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ximilar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ximilar
provider_slug: ximilar
scheme_count: 1
schemes:
- applies_to: all api.ximilar.com services
  in: header
  name: ximilarToken
  note: '"All requests to the Ximilar API must include your API token in the request headers. This applies to all HTTP methods: GET, POST, PUT, and DELETE." Content-Type must be application/json.'
  parameter_name: Authorization
  sources:
  - https://docs.ximilar.com/quickstart
  type: apiKey
  value_format: Token <API_TOKEN>
slug: ximilar-authentication
source_filename: ximilar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://docs.ximilar.com/quickstart\ndocs: https://docs.ximilar.com/quickstart\nprovider: Ximilar\nproviderId: ximilar\ndescription: >-\n  Ximilar uses a single long-lived API token issued per account in the Ximilar App. There\n  is no OAuth 2.0, no OpenID Connect, no mTLS and no scope system; every request on every\n  service carries the same token. Derived from the provider's own Quickstart page, not\n  from a specification — Ximilar publishes no OpenAPI, so there are no securitySchemes to\n  aggregate.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  scopes: none\nschemes:\n  - name: ximilarToken\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    value_format: 'Token <API_TOKEN>'\n    applies_to: all api.ximilar.com services\n    sources: [https://docs.ximilar.com/quickstart]\n    note: >-\n      \"All requests to the Ximilar\
  \ API must include your API token in the request headers.\n      This applies to all HTTP methods: GET, POST, PUT, and DELETE.\" Content-Type must be\n      application/json.\ntoken_management:\n  issue_url: https://app.ximilar.com/my-plan/settings\n  signup_url: https://app.ximilar.com/register\n  rotation_documented: false\n  expiry_documented: false\n  scope_model: none — one account token grants every service the active plan includes\nadditional_request_identity:\n  - header: collection-id\n    applies_to: Visual Search / similarity services\n    description: >-\n      Search and similarity operations address a specific image collection via a\n      collection-id request header rather than a path parameter. Collections must be\n      created by Ximilar administrators before use.\n    source: https://docs.ximilar.com/visual-search/overview\n  - field: workspace\n    applies_to: Computer Vision Platform, VLM, async requests\n    description: Workspace UUID; defaults to the account's\
  \ default workspace when omitted.\nmcp_auth:\n  type: api-key\n  env: XIMILAR_API_KEY\n  note: The local MCP server takes the same account token via an environment variable.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ximilar/refs/heads/main/authentication/ximilar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Computer-Vision
- Image Recognition
- Visual Search
- Image Tagging
- Machine-Learning
- Artificial Intelligence
- OCR
- Collectibles
- Fashion
- E-Commerce
- MCP
- Image Processing
---
