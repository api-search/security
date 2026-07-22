---
api_key_in: []
api_specs:
- filename: usebutton-brands-openapi.yml
  format: yaml
  label: Button Brands API
  slug: button-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-brands-openapi.yml
- filename: usebutton-billing-openapi.yml
  format: yaml
  label: Button Billing API
  slug: button-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-billing-openapi.yml
- filename: usebutton-links-openapi.yml
  format: yaml
  label: Button Links API
  slug: button-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-links-openapi.yml
- filename: usebutton-shortlink-openapi.yml
  format: yaml
  label: Button Shortlink API
  slug: button-shortlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-shortlink-openapi.yml
- filename: usebutton-offers-openapi.yml
  format: yaml
  label: Button Offers API
  slug: button-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/openapi/usebutton-offers-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Usebutton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Button secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Button
provider_slug: usebutton
scheme_count: 1
schemes:
- name: sec0
  scheme: basic
  sources:
  - openapi/usebutton-brands-openapi.yml
  - openapi/usebutton-billing-openapi.yml
  - openapi/usebutton-links-openapi.yml
  - openapi/usebutton-shortlink-openapi.yml
  - openapi/usebutton-offers-openapi.yml
  type: http
  usage: API key as Basic auth username with empty password
slug: usebutton-authentication
source_filename: usebutton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: OpenAPI definitions embedded in https://developer.usebutton.com/reference/* pages + curl code samples\ndocs: https://developer.usebutton.com/reference/getting-started\nsummary:\n  types:\n    - http\n  http_schemes:\n    - basic\n  oauth2_flows: []\n  api_key_in: []\n  notes: >-\n    Every Button server-to-server API (Brands, Billing/Affiliation, Links, Shortlink, Offers,\n    Order) authenticates with HTTP Basic auth using the organization's API key as the username\n    and a blank password (curl -u YOUR_API_KEY:). API keys are issued per organization in the\n    Button Dashboard (https://app.usebutton.com). Webhook callbacks are authenticated in the\n    other direction with an HMAC-SHA256 signature over the raw body in the X-Button-Signature\n    header (see asyncapi/usebutton-webhooks.yml).\nschemes:\n  - name: sec0\n    type: http\n    scheme: basic\n    usage: API key as Basic auth username with empty password\n    sources:\n\
  \      - openapi/usebutton-brands-openapi.yml\n      - openapi/usebutton-billing-openapi.yml\n      - openapi/usebutton-links-openapi.yml\n      - openapi/usebutton-shortlink-openapi.yml\n      - openapi/usebutton-offers-openapi.yml\nrelated:\n  webhooks_signature: asyncapi/usebutton-webhooks.yml\n  conventions: conventions/usebutton-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usebutton/refs/heads/main/authentication/usebutton-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Mobile Commerce
- Affiliate
- Attribution
- Deep Linking
- Offers
- Publishers
- Retail
---
