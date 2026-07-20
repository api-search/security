---
api_key_in:
- header
api_specs:
- filename: blocktorch-hardhat-forking-openapi.yml
  format: yaml
  label: Blocktorch Hardhat Forking API
  slug: blocktorch-hardhat-forking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blocktorch/refs/heads/main/openapi/blocktorch-hardhat-forking-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Blocktorch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blocktorch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blocktorch
provider_slug: blocktorch
scheme_count: 1
schemes:
- description: API key created on the Settings page of your Blocktorch project dashboard. Include it in the header of every request.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/blocktorch-hardhat-forking-openapi.yml
  type: apiKey
slug: blocktorch-authentication
source_filename: blocktorch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/blocktorch-hardhat-forking-openapi.yml\ndocs: https://docs.blocktorch.xyz/concepts/data-sources/local-forks/hardhat-forking-api.md\nnotes: >-\n  API access uses a project-scoped API key passed in the x-api-key header. Keys\n  are created on the Settings page of the Blocktorch project dashboard. Platform\n  (dashboard) sign-in additionally supports email magic-link, Google/GitHub SSO,\n  and Web3 wallet, but those govern the app UI, not the documented API.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key created on the Settings page of your Blocktorch project dashboard. Include\n    it in the header of every request.\n  sources:\n  - openapi/blocktorch-hardhat-forking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blocktorch/refs/heads/main/authentication/blocktorch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Web3
- Observability
- Monitoring
- Blockchain
- Smart Contracts
- dApps
- Developer Tools
---
