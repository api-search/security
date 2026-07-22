---
api_key_in: []
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Urbanremedy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Urban Remedy secures its APIs with none and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Urban Remedy
provider_slug: urbanremedy
scheme_count: 2
schemes:
- description: WooCommerce Store API (wc/store/v1) — public read access to the product catalog; cart/checkout routes use platform-managed Cart-Token session tokens.
  evidence: GET /wp-json/wc/store/v1/products returned 200 with product JSON
  name: public-store-api
  type: none
- description: WooCommerce management REST API (wc/v3) — requires WooCommerce consumer key/secret issued by the store; not a public developer program.
  evidence: GET /wp-json/wc/v3/products returned 401 unauthenticated
  name: woocommerce-rest-keys
  type: apiKey
slug: urbanremedy-authentication
source_filename: urbanremedy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: live probes of https://urbanremedy.com/wp-json/ (2026-07-21)\nsummary:\n  types: [none, apiKey]\n  notes: >-\n    Urban Remedy publishes no developer program of its own; its API surface is\n    the platform-provided WordPress + WooCommerce REST layer at /wp-json/.\n    Access models observed live: the WooCommerce Store API (wc/store/v1) and\n    the WordPress content API (wp/v2 read endpoints) are public and\n    unauthenticated (verified HTTP 200 with JSON payloads); the WooCommerce\n    management REST API (wc/v3) rejects unauthenticated requests (verified\n    HTTP 401) and, per the WooCommerce platform standard, requires store-issued\n    consumer key/secret credentials that are not publicly available.\nschemes:\n- name: public-store-api\n  type: none\n  description: WooCommerce Store API (wc/store/v1) — public read access to the\n    product catalog; cart/checkout routes use platform-managed Cart-Token\n    session tokens.\n\
  \  evidence: GET /wp-json/wc/store/v1/products returned 200 with product JSON\n- name: woocommerce-rest-keys\n  type: apiKey\n  description: WooCommerce management REST API (wc/v3) — requires WooCommerce\n    consumer key/secret issued by the store; not a public developer program.\n  evidence: GET /wp-json/wc/v3/products returned 401 unauthenticated\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanremedy/refs/heads/main/authentication/urbanremedy-authentication.yml
summary_line: none/apiKey · 2 schemes
tags:
- Company
- Food
- Organic
- Plant-Based
- Juice
- Wellness
- eCommerce
- Retail
---
