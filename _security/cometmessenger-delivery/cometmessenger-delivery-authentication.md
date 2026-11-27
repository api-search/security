---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cometmessenger-delivery-book-api-openapi.yml
  format: yaml
  label: Comet Messenger Service Book API
  slug: cometmessenger-delivery-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cometmessenger-delivery/openapi/cometmessenger-delivery-book-api-openapi.yml
- filename: cometmessenger-delivery-orders-api-openapi.yml
  format: yaml
  label: Comet Messenger Service Orders API
  slug: cometmessenger-delivery-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cometmessenger-delivery/openapi/cometmessenger-delivery-orders-api-openapi.yml
- filename: cometmessenger-delivery-quote-api-openapi.yml
  format: yaml
  label: Comet Messenger Service Quote API
  slug: cometmessenger-delivery-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cometmessenger-delivery/openapi/cometmessenger-delivery-quote-api-openapi.yml
- filename: cometmessenger-delivery-status-api-openapi.yml
  format: yaml
  label: Comet Messenger Service Status API
  slug: cometmessenger-delivery-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cometmessenger-delivery/openapi/cometmessenger-delivery-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Comet Messenger Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comet Messenger Service secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Comet Messenger Service
provider_slug: cometmessenger-delivery
scheme_count: 1
schemes:
- applies_to:
  - book_delivery
  - order_status
  - recent_orders
  description: Comet account key (cmt_...). Issued by Comet to account holders.
  header_text: 'Account keys: send as `Authorization: Bearer cmt_...`.'
  issuance: Comet account holders can ask for a key for their firm's AI agent at (312) 786-2288.
  key_prefix: cmt_
  name: accountKey
  scheme: bearer
  sources:
  - openapi/cometmessenger-delivery-openapi.yml
  - https://cometmessenger.delivery/llms.txt
  type: http
slug: cometmessenger-delivery-authentication
source_filename: cometmessenger-delivery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cometmessenger.delivery/llms.txt\ndocs: https://cometmessenger.delivery/llms.txt\nsummary:\n  types:\n  - http\nschemes:\n- name: accountKey\n  type: http\n  scheme: bearer\n  description: Comet account key (cmt_...). Issued by Comet to account holders.\n  key_prefix: cmt_\n  header_text: \"Account keys: send as `Authorization: Bearer cmt_...`.\"\n  issuance: \"Comet account holders can ask for a key for their firm's AI agent at (312) 786-2288.\"\n  applies_to: [book_delivery, order_status, recent_orders]\n  sources:\n  - openapi/cometmessenger-delivery-openapi.yml\n  - https://cometmessenger.delivery/llms.txt\nanonymous_operations:\n- operation: get_quote\n  note: \"`get_quote` (no sign-in) - POST /quote\"\nself_service_keys: false\nnote: Keys are issued by phone to existing account holders; there is no self-service key console, OAuth flow or scope model documented.\n"
source_yaml_url: https://artifacts.apis.io/cometmessenger-delivery/authentication/cometmessenger-delivery-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Couriers
- Same-Day Delivery
- Logistics
- Chicago
- Delivery
- MCP
---
