---
anonymous_access: true
api_key_in: []
api_specs:
- filename: costsegsmart-com-openapi-generated.yml
  format: yaml
  label: Cost Seg Smart API
  slug: costsegsmart-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costsegsmart-com/openapi/_ae-authored/costsegsmart-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cost Seg Smart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cost Seg Smart declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cost Seg Smart
provider_slug: costsegsmart-com
scheme_count: 2
schemes:
- description: '"`/api/quote` is open." No credential is documented for /api/quote, /api/product-feed.json or /api/payment-link.'
  type: none
- applies_to:
  - post_api_payment_link
  description: '"`/api/payment-link` may require a buyer email or Cloudflare Turnstile challenge if the calling IP doesn''t have a recognized agent UA".'
  name: Cloudflare Turnstile
  type: challenge
slug: costsegsmart-com-authentication
source_filename: costsegsmart-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://costsegsmart.com/llms-commerce.txt\ndocs: https://costsegsmart.com/llms-commerce.txt\nsummary: The agent-commerce endpoints are unauthenticated; no API key or OAuth is documented. Callers are identified by an optional X-Agent-Name header and by user-agent (which sets the rate-limit tier). /api/payment-link may additionally demand a buyer email or a Cloudflare Turnstile challenge for callers without a recognized agent user-agent.\nschemes:\n- type: none\n  description: '\"`/api/quote` is open.\" No credential is documented for /api/quote, /api/product-feed.json or /api/payment-link.'\n- type: challenge\n  name: Cloudflare Turnstile\n  applies_to: [post_api_payment_link]\n  description: '\"`/api/payment-link` may require a buyer email or Cloudflare Turnstile challenge if the calling IP doesn''t have a recognized agent UA\".'\nheaders:\n- name: X-Agent-Name\n  in: header\n  required: false\n  description: Agent identifier;\
  \ recommended, appears in the Stripe Checkout disclaimer.\n"
source_yaml_url: https://artifacts.apis.io/costsegsmart-com/authentication/costsegsmart-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cost Segregation
- Tax
- Depreciation
- Real Estate
- Accounting
- MCP
- Agentic Commerce
---
