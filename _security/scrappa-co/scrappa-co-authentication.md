---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Scrappa Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: scrappa-co declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: scrappa-co
provider_slug: scrappa-co
scheme_count: 2
schemes:
- description: API key for account-based credits
  in: header
  name: X-API-KEY
  type: apiKey
- description: Accountless payment via x402 on Base (USDC)
  type: x402
slug: scrappa-co-authentication
source_filename: scrappa-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://scrappa.co/docs/authentication\nschemes:\n  - type: apiKey\n    name: X-API-KEY\n    in: header\n    description: API key for account-based credits\n  - type: x402\n    description: Accountless payment via x402 on Base (USDC)\n"
source_yaml_url: https://artifacts.apis.io/scrappa-co/authentication/scrappa-co-authentication.yml
summary_line: 2 schemes
tags:
- Web Scraping
- Data API
- Search
- Automation
- JSON
- API
---
