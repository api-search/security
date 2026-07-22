---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Storehub Authentication
name_suffix: Authentication
oauth_flows: []
overview: StoreHub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StoreHub
provider_slug: storehub
scheme_count: 1
schemes:
- description: HTTP Basic-style credentials (Consumer Username + Secret / API token) issued by StoreHub Customer Care on request. Presented per-request to the merchant's BackOffice host ([storename].storehubhq.com). No OAuth2 or OpenID Connect surface is published.
  gated: true
  name: apiToken
  request_via: https://care.storehub.com/en/
  scheme: basic
  sources: []
  type: http
slug: storehub-authentication
source_filename: storehub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://care.storehub.com/en/articles/5727084-financio-how-to-integrate-with-storehub\ndocs: https://care.storehub.com/en/\nsummary:\n  types: [http]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    StoreHub operates a private, partner-gated REST API. There is no public\n    OpenAPI specification or self-serve developer portal. API credentials\n    (documented across partner integration guides as an \"API token\" /\n    \"Consumer Username & Secret\") must be requested from StoreHub Customer\n    Care. Dedicated API access is described as an Enterprise-tier feature.\nschemes:\n- name: apiToken\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic-style credentials (Consumer Username + Secret / API token)\n    issued by StoreHub Customer Care on request. Presented per-request to the\n    merchant's BackOffice host ([storename].storehubhq.com). No OAuth2 or\n    OpenID Connect surface is published.\n  gated:\
  \ true\n  request_via: https://care.storehub.com/en/\n  sources: []\nhosts:\n- pattern: https://<storename>.storehubhq.com\n  note: Per-merchant BackOffice host; the API is scoped to the merchant account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storehub/refs/heads/main/authentication/storehub-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Point of Sale
- Retail
- Restaurant
- Inventory Management
- Payments
- E-commerce
- Loyalty
- Southeast Asia
- Small Business
---
