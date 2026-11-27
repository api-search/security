---
anonymous_access: false
api_key_in: []
api_specs:
- filename: abstraxn-com-ai-openapi-generated.yml
  format: yaml
  label: Abstraxn ai API
  slug: ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abstraxn-com/openapi/_ae-authored/abstraxn-com-ai-openapi-generated.yml
- filename: abstraxn-com-kyi-openapi-generated.yml
  format: yaml
  label: Abstraxn kyi API
  slug: kyi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abstraxn-com/openapi/_ae-authored/abstraxn-com-kyi-openapi-generated.yml
- filename: abstraxn-com-wallets-openapi-generated.yml
  format: yaml
  label: Abstraxn wallets API
  slug: wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abstraxn-com/openapi/_ae-authored/abstraxn-com-wallets-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Abstraxn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abstraxn declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Abstraxn
provider_slug: abstraxn-com
scheme_count: 2
schemes:
- description: Application API key provided from dashboard, used for initial authentication
  in: header
  name: API Key
  type: apiKey
- description: JWT access token obtained after authentication flow
  scheme: Bearer
  type: bearer
slug: abstraxn-com-authentication
source_filename: abstraxn-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.abstraxn.com/guides/wallets/server-wallet/authentication.md\nschemes:\n  - type: apiKey\n    name: \"API Key\"\n    in: header\n    description: \"Application API key provided from dashboard, used for initial authentication\"\n  - type: bearer\n    scheme: \"Bearer\"\n    description: \"JWT access token obtained after authentication flow\"\n"
source_yaml_url: https://artifacts.apis.io/abstraxn-com/authentication/abstraxn-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Agents
- Payments
- Identity
- Wallets
- Web3
- Technology
---
