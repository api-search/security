---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Voltage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voltage secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Voltage
provider_slug: voltage
scheme_count: 2
schemes:
- description: Environment-scoped Payments API key. Generated from the team "API Keys" page in the Voltage dashboard; each key is bound to one environment so staging and production can be separated cleanly. Sent on every request as the x-api-key header.
  in: header
  name: PaymentsApiKey
  parameter: x-api-key
  sources:
  - https://docs.voltageapi.com/developer-guide
  - https://docs.voltageapi.com/payments-access
  type: apiKey
- description: Separate key for the Infrastructure API (node lifecycle/management). Created from the Infrastructure dashboard by a team member with Write access. Does not bypass node password or LND macaroon permissions.
  in: header
  name: InfrastructureApiKey
  parameter: x-api-key
  sources:
  - https://docs.voltageapi.com/access-model
  type: apiKey
slug: voltage-authentication
source_filename: voltage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.voltageapi.com/developer-guide\ndocs: https://docs.voltageapi.com/security\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: PaymentsApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    Environment-scoped Payments API key. Generated from the team \"API Keys\" page in\n    the Voltage dashboard; each key is bound to one environment so staging and\n    production can be separated cleanly. Sent on every request as the x-api-key\n    header.\n  sources: [https://docs.voltageapi.com/developer-guide, https://docs.voltageapi.com/payments-access]\n- name: InfrastructureApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    Separate key for the Infrastructure API (node lifecycle/management). Created from\n    the Infrastructure dashboard by a team member with Write access. Does not bypass\n    node password or LND macaroon\
  \ permissions.\n  sources: [https://docs.voltageapi.com/access-model]\nnode_access:\n- name: LND Macaroons\n  type: macaroon\n  description: >-\n    LND-native credentials for direct node access (REST/gRPC/lncli), separate from\n    Voltage team permissions and API keys. Types include admin/super-admin,\n    read-only, invoice, and custom baked macaroons. Encrypted macaroon material is\n    decrypted with the node password; exported/decrypted macaroons must be treated\n    as secrets.\n  docs: https://docs.voltageapi.com/macaroons\nnotes: >-\n  The Voltage Payments API is key-authenticated (x-api-key), not OAuth2/OIDC, so there\n  is no OAuth scope surface (scopes/ artifact intentionally omitted). Permission\n  layering is documented under the Access Model, Node Security, and Macaroons pages.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltage/refs/heads/main/authentication/voltage-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Enterprise
- Bitcoin
- Lightning Network
- Payments
- Cryptocurrency
- Financial Services
- Wallets
- Infrastructure
- Fintech
- Node Hosting
- Web3
---
