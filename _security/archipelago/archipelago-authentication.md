---
api_key_in: []
auth_types:
- credential
description: ''
kind: authentication
layout: security
method: searched
name: Archipelago Authentication
name_suffix: Authentication
oauth_flows: []
overview: Archipelago secures its APIs with credential across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Archipelago
provider_slug: archipelago
scheme_count: 1
schemes:
- description: Customer-specific credentials issued by Archipelago, presented when calling the GraphQL API. Exact header/parameter name is documented behind the authenticated developer docs.
  name: ArchipelagoAPICredentials
  sources:
  - https://docs.onarchipelago.com/api
  type: apiKey
slug: archipelago-authentication
source_filename: archipelago-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.onarchipelago.com/api\ndocs: https://docs.onarchipelago.com/api\nnotes: >-\n  Archipelago's public-facing API is a GraphQL API. Per Archipelago's documentation, access is\n  credential-based: Archipelago provisions credentials to customers, who use them to authenticate\n  to the Archipelago API. The API reference and the exact credential/header mechanics sit behind\n  the authenticated platform (docs.onarchipelago.com/api requires a magic-link login), so the\n  low-level scheme details are not publicly enumerable. No public OpenAPI is published; this\n  profile is derived from Archipelago's published statements about API access, not a machine-read\n  security scheme. The end-user platform (platform.onarchipelago.com) itself signs users in via a\n  passwordless magic-link email flow.\nsummary:\n  types:\n  - credential\n  api_style: graphql\n  credential_provisioning: customer-provisioned-by-vendor\n  public_openapi:\
  \ false\nschemes:\n- name: ArchipelagoAPICredentials\n  type: apiKey\n  description: >-\n    Customer-specific credentials issued by Archipelago, presented when calling the GraphQL API.\n    Exact header/parameter name is documented behind the authenticated developer docs.\n  sources:\n  - https://docs.onarchipelago.com/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archipelago/refs/heads/main/authentication/archipelago-authentication.yml
summary_line: credential · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Property Risk
- Underwriting
- Risk Management
- Commercial Property
- GraphQL
- Data
- AI Agent
---
