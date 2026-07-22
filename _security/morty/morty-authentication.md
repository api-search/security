---
api_key_in:
- unknown
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Morty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Morty secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Morty
provider_slug: morty
scheme_count: 1
schemes:
- description: Morty provisions an API key for its embeddable mortgage widgets / Product & Pricing Engine. The key is issued through Contact Sales as part of a partnership ("Get your API key for Morty's embeddable mortgage widgets"). No public OpenAPI, developer portal, or auth reference documents the key placement (header vs. query), so `in`/parameter name are unknown.
  name: apiKey
  sources:
  - https://platform.morty.com/contact-sales/
  type: apiKey
slug: morty-authentication
source_filename: morty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://platform.morty.com/contact-sales/\nsummary:\n  types: [apiKey]\n  api_key_in: [unknown]\n  oauth2_flows: []\n  public_spec: false\n  access: partner-gated\nschemes:\n  - name: apiKey\n    type: apiKey\n    description: >-\n      Morty provisions an API key for its embeddable mortgage widgets / Product &\n      Pricing Engine. The key is issued through Contact Sales as part of a\n      partnership (\"Get your API key for Morty's embeddable mortgage widgets\").\n      No public OpenAPI, developer portal, or auth reference documents the key\n      placement (header vs. query), so `in`/parameter name are unknown.\n    sources: [https://platform.morty.com/contact-sales/]\nnotes: >-\n  Authentication details are behind a partner onboarding / Contact Sales flow;\n  Morty publishes no public API reference. Recorded from the documented fact that\n  API keys are issued for the embeddable widgets and PPE-over-API surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morty/refs/heads/main/authentication/morty-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Mortgage
- Lending
- Fintech
- Mortgage Infrastructure
- Loan Origination
- Pricing Engine
- Embedded Finance
- API
---
