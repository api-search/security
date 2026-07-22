---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Okendo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Okendo secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Okendo
provider_slug: okendo
scheme_count: 2
schemes:
- applies_to: Merchant (Enterprise) REST API
  credential: base64("<okendo_user_id>:<api_key>")
  header: 'Authorization: Basic <base64-credentials>'
  key_source: Okendo app > integration settings
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.okendo.io/merchant-rest-api/quick-start
  type: http
- applies_to: Storefront REST API
  name: publicStorefront
  notes: Public read-only endpoints scoped by okendo_user_id path segment; no credential required.
  scheme: none
  sources:
  - https://docs.okendo.io/on-site/storefront-rest-api/quick-start
  type: none
slug: okendo-authentication
source_filename: okendo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.okendo.io/merchant-rest-api/quick-start\ndocs: https://docs.okendo.io/merchant-rest-api/quick-start\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Okendo exposes two REST surfaces with different auth models. The Merchant\n    (Enterprise) REST API uses HTTP Basic authentication; credentials are the\n    Okendo user id and API key combined as \"<okendo_user_id>:<api_key>\" and\n    base64-encoded, obtained from the integration settings section of the Okendo\n    app. All requests must also send an okendo-api-version date header. The\n    Storefront REST API is a public, unauthenticated read surface scoped by\n    okendo_user_id in the path.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  applies_to: Merchant (Enterprise) REST API\n  credential: base64(\"<okendo_user_id>:<api_key>\")\n  header: 'Authorization: Basic <base64-credentials>'\n\
  \  key_source: Okendo app > integration settings\n  sources: [https://docs.okendo.io/merchant-rest-api/quick-start]\n- name: publicStorefront\n  type: none\n  scheme: none\n  applies_to: Storefront REST API\n  notes: Public read-only endpoints scoped by okendo_user_id path segment; no credential required.\n  sources: [https://docs.okendo.io/on-site/storefront-rest-api/quick-start]\nversion_header:\n  name: okendo-api-version\n  required: true\n  example: '2025-02-01'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okendo/refs/heads/main/authentication/okendo-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Business Applications
- Reviews
- Ratings
- Ecommerce
- Loyalty
- Customer Marketing
- Shopify
- Webhooks
---
