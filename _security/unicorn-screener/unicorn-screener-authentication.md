---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Unicorn Screener API
  slug: unicorn-screener-api
  spec_type: OpenAPI
  url: https://unicornscreener.vc/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Unicorn Screener Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unicorn Screener declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Unicorn Screener
provider_slug: unicorn-screener
scheme_count: 0
schemes: []
slug: unicorn-screener-authentication
source_filename: unicorn-screener-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: derived\nsource: >-\n  Derived from openapi/unicorn-screener-openapi.json (security:[], no securitySchemes)\n  and confirmed against https://unicornscreener.vc/docs/ai-agents (\"No API key required\",\n  \"No CAPTCHA No Auth Required\"). Confirmed live: GET /api/agent/lookup?name=Stripe\n  returned 200 JSON with no credentials.\ntype: none\nschemes: []\ndetail: >-\n  Public keyless HTTP JSON API. No API key, bearer token, OAuth, OpenID Connect or mutual\n  TLS is required or offered. All four operations are callable anonymously.\nidentity_signals:\n  purpose: quota enforcement only, not authentication\n  fields:\n  - email (for the screening request and memo delivery)\n  - fingerprint (stable persisted caller identifier)\n  - cookie (existing visitor cookie)\n  guidance: Reuse these consistently across calls; never rotate email/fingerprint/cookie/IP to evade limits.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicorn-screener/refs/heads/main/authentication/unicorn-screener-authentication.yml
summary_line: 0 schemes
tags:
- Venture Capital
- Startups
- Company Research
- Screening
- Investing
- AI Agents
---
