---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cratejoy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cratejoy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cratejoy
provider_slug: cratejoy
scheme_count: 1
schemes:
- applies_to: Merchant API (https://api.cratejoy.com/v1/)
  credentials:
  - Client ID
  - Client Secret Key
  description: 'The Cratejoy Merchant API uses HTTP Basic authentication. You Base64-encode your API credentials as `client_id:client_secret` and pass them in the Authorization header (Authorization: Basic {base64(client_id:client_secret)}).'
  name: basicAuth
  obtain: Admin users generate API keys from the merchant dashboard under Settings > API. Non-admin roles (Customer Support, Developers) cannot access this panel and must request key generation from a store administrator.
  scheme: basic
  sources:
  - docs.cratejoy.com/reference/authorization
  type: http
slug: cratejoy-authentication
source_filename: cratejoy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cratejoy.com/reference/authorization\ndocs: https://docs.cratejoy.com/reference/authorization\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      The Cratejoy Merchant API uses HTTP Basic authentication. You Base64-encode\n      your API credentials as `client_id:client_secret` and pass them in the\n      Authorization header (Authorization: Basic {base64(client_id:client_secret)}).\n    credentials:\n      - Client ID\n      - Client Secret Key\n    obtain: >-\n      Admin users generate API keys from the merchant dashboard under Settings > API.\n      Non-admin roles (Customer Support, Developers) cannot access this panel and must\n      request key generation from a store administrator.\n    applies_to: Merchant API (https://api.cratejoy.com/v1/)\n    sources: [docs.cratejoy.com/reference/authorization]\n\
  notes: >-\n  The Store API is a separate surface that reads (and sometimes writes) data on behalf\n  of the logged-in customer from front-end JavaScript, rather than using Basic API\n  credentials. No OAuth2/OIDC surface is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cratejoy/refs/heads/main/authentication/cratejoy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ecommerce
- Subscriptions
- Subscription Boxes
- Marketplace
- Payments
- Orders
- Webhooks
- REST
---
