---
api_key_in:
- header
api_specs:
- filename: ship24-tracking-api.yaml
  format: yaml
  label: Ship24 Tracking API
  slug: ship24-tracking-api
  spec_type: OpenAPI
  url: https://docs.ship24.com/assets/openapi/ship24-tracking-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ship24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ship24 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ship24
provider_slug: ship24
scheme_count: 1
schemes:
- description: 'The Ship24 API uses API keys to authenticate requests. You can [view and manage them in your Dashboard](https://dashboard.ship24.com/integrations/api-keys). A `Default` API key is created after you subscribe to a plan.


    To authenticate your requests, include an `Authorization` HTTP header to all your requests with the following value: `Bearer your_api_key`. (Replace `your_api_key` by the one from '
  in: header
  name: Authorization
  parameter: Bearer your_api_key
  sources:
  - openapi/ship24-tracking-api-openapi.yml
  type: apiKey
slug: ship24-authentication
source_filename: ship24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ship24-tracking-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Bearer your_api_key\n  description: \"The Ship24 API uses API keys to authenticate requests. You can [view and manage\\\n    \\ them in your Dashboard](https://dashboard.ship24.com/integrations/api-keys). A `Default`\\\n    \\ API key is created after you subscribe to a plan.\\n\\nTo authenticate your requests, include\\\n    \\ an `Authorization` HTTP header to all your requests with the following value: `Bearer\\\n    \\ your_api_key`. (Replace `your_api_key` by the one from \"\n  sources:\n  - openapi/ship24-tracking-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ship24/refs/heads/main/authentication/ship24-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Tracking
- Logistics
- Shipping
- Couriers
- Parcels
- Webhooks
- Ecommerce
- PostPurchase
---
