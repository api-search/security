---
api_key_in: []
auth_types:
- apiKey
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Dewu Poizon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dewu (POIZON) secures its APIs with apiKey and signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dewu (POIZON)
provider_slug: dewu-poizon
scheme_count: 1
schemes:
- authorization_models:
  - Seller authentication (open.poizon.com/doc/list/documentationDetail/9)
  - ISV / ERP authorization
  description: Requests are identified by an application app_key and signed with a computed request signature (the docs reference a "Sign" method and a hosted "Sign Tool"). Sellers and ISV/ERP integrators are authorized to obtain credentials through the Open Platform before calling the API.
  name: AppKeySignature
  parameters:
  - app_key
  - sign
  type: apiKey
slug: dewu-poizon-authentication
source_filename: dewu-poizon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://open.poizon.com/doc/list/documentationDetail/9\ndocs:\n- https://open.poizon.com/doc/list/documentationDetail/9\n- https://open.poizon.com/doc/list/documentationDetail/15\nnotes: >-\n  Captured from the POIZON / Dewu Open Platform (open.poizon.com, open.dewu.com)\n  developer documentation. The portal is a JS-rendered SPA and geo-restricted, so\n  a full securityScheme could not be harvested; the model below reflects what the\n  published docs navigation and authentication pages describe. No OpenAPI is\n  published, so this is not derived from a spec.\nsummary:\n  types:\n  - apiKey\n  - signature\n  model: app-key + request signature (HMAC sign) — common Chinese open-platform pattern\nschemes:\n- name: AppKeySignature\n  type: apiKey\n  description: >-\n    Requests are identified by an application app_key and signed with a computed\n    request signature (the docs reference a \"Sign\" method and a hosted \"Sign Tool\"\
  ).\n    Sellers and ISV/ERP integrators are authorized to obtain credentials through the\n    Open Platform before calling the API.\n  parameters:\n  - app_key\n  - sign\n  authorization_models:\n  - Seller authentication (open.poizon.com/doc/list/documentationDetail/9)\n  - ISV / ERP authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dewu-poizon/refs/heads/main/authentication/dewu-poizon-authentication.yml
summary_line: apiKey/signature · 1 scheme
tags:
- Company
- Technology
- E-Commerce
- Marketplace
- Retail
- Sneakers
- Luxury Goods
- Authentication
- China
---
