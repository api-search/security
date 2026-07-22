---
api_key_in: []
api_specs:
- filename: nine-fives-attenuator-openapi.yml
  format: yaml
  label: Nine Fives Programmable Attenuator API
  slug: nine-fives-programmable-attenuator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nine-fives/refs/heads/main/openapi/nine-fives-attenuator-openapi.yml
- filename: nine-fives-switch-openapi.yml
  format: yaml
  label: Nine Fives Programmable SPDT Switch API
  slug: nine-fives-programmable-spdt-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nine-fives/refs/heads/main/openapi/nine-fives-switch-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Nine Fives Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nine Fives secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nine Fives
provider_slug: nine-fives
scheme_count: 0
schemes: []
slug: nine-fives-authentication
source_filename: nine-fives-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.ninefives.com/attenuator/rest-api/overview/\nsummary:\n  types: [none]\n  note: >-\n    The Nine Fives device REST API (attenuator and SPDT switch) is served directly\n    by the instrument on the local network (Ethernet / USB-C) on port 80 and\n    documents NO authentication — access control is the local network boundary,\n    consistent with lab-bench RF test instruments. SCPI over TCP (5025) and HiSLIP\n    (4880) are likewise unauthenticated. Deployments should isolate devices on a\n    trusted test LAN.\nschemes: []\nstorefront_auth:\n  note: >-\n    Separately, the ninefives.com Shopify storefront exposes customer-account\n    OpenID Connect (issuer https://shopify.com/authentication/77424886003) for\n    shopper login — this governs the store, not the device API.\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/77424886003\n  scopes_supported: [openid, email, customer-account-api:full,\
  \ customer-account-mcp-api:full]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nine-fives/refs/heads/main/authentication/nine-fives-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- RF Test Equipment
- Test and Measurement
- Hardware
- IoT
- Instrumentation
- Automation
- Aerospace
- Attenuator
- RF Switch
- SCPI
---
