---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nibgate-xyz-discovery-api-openapi.yml
  format: yaml
  label: Nibgate Discovery API
  slug: nibgate-xyz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-discovery-api-openapi.yml
- filename: nibgate-xyz-jev-api-openapi.yml
  format: yaml
  label: Nibgate JEV API
  slug: nibgate-xyz-jev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-jev-api-openapi.yml
- filename: nibgate-xyz-ledger-api-openapi.yml
  format: yaml
  label: Nibgate Ledger API
  slug: nibgate-xyz-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-ledger-api-openapi.yml
- filename: nibgate-xyz-platform-api-openapi.yml
  format: yaml
  label: Nibgate Platform API
  slug: nibgate-xyz-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-platform-api-openapi.yml
- filename: nibgate-xyz-reputation-api-openapi.yml
  format: yaml
  label: Nibgate Reputation API
  slug: nibgate-xyz-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-reputation-api-openapi.yml
- filename: nibgate-xyz-tips-api-openapi.yml
  format: yaml
  label: Nibgate Tips API
  slug: nibgate-xyz-tips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-tips-api-openapi.yml
- filename: nibgate-xyz-unlocks-api-openapi.yml
  format: yaml
  label: Nibgate Unlocks API
  slug: nibgate-xyz-unlocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-unlocks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nibgate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nibgate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nibgate
provider_slug: nibgate-xyz
scheme_count: 1
schemes:
- description: x402 payment challenge-response header. Include the header on retry after settlement to unlock paid content.
  in: header
  name: x402
  parameter: Payment
  sources:
  - openapi/nibgate-xyz-openapi.json
  type: apiKey
slug: nibgate-xyz-authentication
source_filename: nibgate-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nibgate-xyz-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: Payment\n  description: x402 payment challenge-response header. Include the header on retry after settlement\n    to unlock paid content.\n  sources:\n  - openapi/nibgate-xyz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nibgate-xyz/authentication/nibgate-xyz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Paid Content
- USDC
- Arc
- Content Discovery
---
