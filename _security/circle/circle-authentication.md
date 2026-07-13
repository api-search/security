---
api_key_in: []
api_specs:
- filename: developer-controlled-wallets.yaml
  format: yaml
  label: Developer-Controlled Wallets
  slug: developer-controlled-wallets
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/developer-controlled-wallets.yaml
- filename: user-controlled-wallets.yaml
  format: yaml
  label: User-Controlled Wallets
  slug: user-controlled-wallets
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/user-controlled-wallets.yaml
- filename: cctp.yaml
  format: yaml
  label: Cross-Chain Transfer Protocol (CCTP)
  slug: cctp
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/cctp.yaml
- filename: gateway.yaml
  format: yaml
  label: Circle Gateway
  slug: gateway
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/gateway.yaml
- filename: smart-contract-platform.yaml
  format: yaml
  label: Smart Contract Platform
  slug: smart-contract-platform
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/smart-contract-platform.yaml
- filename: cpn-ofi.yaml
  format: yaml
  label: Circle Payments Network (CPN)
  slug: cpn
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/cpn-ofi.yaml
- filename: compliance.yaml
  format: yaml
  label: Compliance Engine
  slug: compliance-engine
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/compliance.yaml
- filename: stablefx.yaml
  format: yaml
  label: StableFX
  slug: stablefx
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/stablefx.yaml
- filename: xreserve.yaml
  format: yaml
  label: xReserve
  slug: xreserve
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/xreserve.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Circle
provider_slug: circle
scheme_count: 1
schemes:
- description: Circle API key, formatted as `PREFIX:ID:SECRET`, supplied as Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/circle-openapi.yml
  type: http
slug: circle-authentication
source_filename: circle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Circle API key, formatted as `PREFIX:ID:SECRET`, supplied as Bearer token.\n  sources:\n  - openapi/circle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/authentication/circle-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Compliance
- Cross-Chain
- Currency
- Money
- Payments
- Stablecoin
- Transfers
- USDC
- Wallets
---
