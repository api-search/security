---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Monetizenow Authentication
name_suffix: Authentication
oauth_flows: []
overview: MonetizeNow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MonetizeNow
provider_slug: monetizenow
scheme_count: 1
schemes:
- description: The preferred (and documented) authentication method is a tenant-generated API key sent in the x-api-key request header. Keys are created in the MonetizeNow tenant under Settings -> API Keys ("New Api Key"), named, and displayed only once at creation. A single key authenticates against all MonetizeNow REST APIs.
  in: header
  name: apiKey
  parameter_name: x-api-key
  provisioning: MonetizeNow tenant UI (Settings -> API Keys)
  sources:
  - https://docs.monetizenow.io/reference/getting-started-with-your-api
  type: apiKey
slug: monetizenow-authentication
source_filename: monetizenow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.monetizenow.io/reference/getting-started-with-your-api\ndocs: https://docs.monetizenow.io/docs/api-keys\nbase_url: https://api.monetizeplatform.com\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    The preferred (and documented) authentication method is a tenant-generated\n    API key sent in the x-api-key request header. Keys are created in the\n    MonetizeNow tenant under Settings -> API Keys (\"New Api Key\"), named, and\n    displayed only once at creation. A single key authenticates against all\n    MonetizeNow REST APIs.\n  provisioning: MonetizeNow tenant UI (Settings -> API Keys)\n  sources:\n  - https://docs.monetizenow.io/reference/getting-started-with-your-api\nnotes:\n- No OAuth 2.0 / OpenID Connect flow is documented for the public REST API; the\n  application UI\
  \ (app.monetizeplatform.com) uses separate interactive login.\n- No public test-vs-live key prefix scheme is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monetizenow/refs/heads/main/authentication/monetizenow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Monetization
- Billing
- Subscriptions
- Usage-Based Pricing
- Quote-to-Cash
- CPQ
- Payments
- Invoicing
- Revenue
- SaaS
- FinTech
---
