---
anonymous_access: false
api_key_in: []
api_specs:
- filename: altcoinchasershq-app-agent-api-openapi.yml
  format: yaml
  label: Altcoin Chasers HQ Agent API
  slug: altcoinchasershq-app-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/altcoinchasershq-app/openapi/altcoinchasershq-app-agent-api-openapi.yml
- filename: altcoinchasershq-app-member-api-openapi.yml
  format: yaml
  label: Altcoin Chasers HQ Member API
  slug: altcoinchasershq-app-member-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/altcoinchasershq-app/openapi/altcoinchasershq-app-member-api-openapi.yml
- filename: altcoinchasershq-app-x402-api-openapi.yml
  format: yaml
  label: Altcoin Chasers HQ X402 API
  slug: altcoinchasershq-app-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/altcoinchasershq-app/openapi/altcoinchasershq-app-x402-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Altcoinchasershq App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Altcoin Chasers HQ secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Altcoin Chasers HQ
provider_slug: altcoinchasershq-app
scheme_count: 2
schemes:
- bearerFormat: hq_live API key
  description: Paid member API key.
  name: memberBearer
  scheme: bearer
  sources:
  - openapi/altcoinchasershq-app-openapi.json
  type: http
- description: Circle Gateway USDC payment.
  name: x402
  scheme: x402
  sources:
  - openapi/altcoinchasershq-app-openapi.json
  type: http
slug: altcoinchasershq-app-authentication
source_filename: altcoinchasershq-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/altcoinchasershq-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: memberBearer\n  type: http\n  scheme: bearer\n  bearerFormat: hq_live API key\n  description: Paid member API key.\n  sources:\n  - openapi/altcoinchasershq-app-openapi.json\n- name: x402\n  type: http\n  scheme: x402\n  description: Circle Gateway USDC payment.\n  sources:\n  - openapi/altcoinchasershq-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/altcoinchasershq-app/authentication/altcoinchasershq-app-authentication.yml
summary_line: http · 2 schemes
tags:
- Cryptocurrency
- Research
- Artificial Intelligence
- Finance
- Altcoins
---
