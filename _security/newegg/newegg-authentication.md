---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Newegg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Newegg secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Newegg
provider_slug: newegg
scheme_count: 3
schemes:
- description: The seller's Newegg Marketplace API Key.
  in: header
  name: Authorization
  parameter: Authorization
  type: apiKey
- description: The seller's Newegg Marketplace Secret Key, paired with the API Key.
  in: header
  name: SecretKey
  parameter: SecretKey
  type: apiKey
- description: The seller account identifier scoping the request to a marketplace seller.
  in: query
  name: sellerid
  parameter: sellerid
  type: apiKey
slug: newegg-authentication
source_filename: newegg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.newegg.com/newegg_marketplace_api/\ndocs: https://developer.newegg.com/newegg_marketplace_api/newegg-developers-quick-guide/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Static credential authentication. There is no OAuth2/OIDC surface. Each\n    request carries two custom headers plus the seller identifier as a query\n    parameter. API Key and Secret Key are issued to registered marketplace\n    sellers (request via Datafeeds@newegg.com).\nschemes:\n  - name: Authorization\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: The seller's Newegg Marketplace API Key.\n  - name: SecretKey\n    type: apiKey\n    in: header\n    parameter: SecretKey\n    description: The seller's Newegg Marketplace Secret Key, paired with the API Key.\n  - name: sellerid\n    type: apiKey\n    in: query\n    parameter: sellerid\n    description: >-\n \
  \     The seller account identifier scoping the request to a marketplace seller.\ncommon_headers:\n  Content-Type: application/json  # application/xml also supported\n  Accept: application/json        # application/xml also supported\nplatforms:\n  - name: Newegg.com (US)\n    host: https://api.newegg.com/marketplace/\n  - name: NeweggBusiness.com (B2B)\n    host: https://api.newegg.com/marketplace/\n  - name: Newegg.ca (Canada)\n    host: https://api.newegg.com/marketplace/\nnotes: >-\n  Resource URL and credentials differ per Newegg platform (US / Business / CA);\n  the API host is api.newegg.com for all three, distinguished by seller\n  credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newegg/refs/heads/main/authentication/newegg-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Consumer
- E-Commerce
- Marketplace
- Retail
- Electronics
- Sellers
- Order Management
- Fulfillment
---
