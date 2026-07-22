---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cooklist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cooklist secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cooklist
provider_slug: cooklist
scheme_count: 2
schemes:
- description: B2B Partner API key mode for authenticating a retailer/partner integration.
  in: header
  name: apiKey
  sources:
  - https://cooklist.com/llms.txt
  type: apiKey
- bearerFormat: JWT
  description: JWT token mode for the B2B Partner API; the embedded SDK obtains session tokens via a retailer-controlled token-mint mechanism.
  name: jwt
  scheme: bearer
  sources:
  - https://cooklist.com/llms.txt
  type: http
slug: cooklist-authentication
source_filename: cooklist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://cooklist.com/llms.txt\ndocs: https://cooklist.com/platform/agentic-commerce\n# Derived from the documented integration model in the platform docs / llms.txt.\n# Cooklist publishes no public OpenAPI, so this is a docs-searched auth profile\n# rather than a spec derivation.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  model: B2B Partner API with per-organization field allowlists (deny-by-default, token-scoped)\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: B2B Partner API key mode for authenticating a retailer/partner integration.\n  sources: [https://cooklist.com/llms.txt]\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token mode for the B2B Partner API; the embedded SDK obtains session tokens via a retailer-controlled token-mint mechanism.\n  sources: [https://cooklist.com/llms.txt]\naccess_controls:\n- Per-organization\
  \ field allowlists restrict each retailer to the capabilities and data scoped to their integration.\n- Deny-by-default, token-scoped access with tenant isolation enforced at app and DB layers.\n- Signed / scoped session tokens prevent user impersonation; tool access is allow-listed (no open web browsing).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooklist/refs/heads/main/authentication/cooklist-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Agentic Commerce
- Grocery
- Retail
- AI Assistant
- Model Context Protocol
- Recipes
- Meal Planning
- E-Commerce
- Personalization
---
