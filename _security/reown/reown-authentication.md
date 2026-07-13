---
api_key_in:
- query
api_specs:
- filename: reown-openapi.yml
  format: yaml
  label: Reown Cloud Explorer API
  slug: explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reown/refs/heads/main/openapi/reown-openapi.yml
- filename: reown-asyncapi.yml
  format: yaml
  label: WalletConnect Relay (SDK-mediated)
  slug: walletconnect-protocol
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/reown/refs/heads/main/asyncapi/reown-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reown Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reown secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reown
provider_slug: reown
scheme_count: 1
schemes:
- description: 'Reown project ID from the Reown Dashboard at

    https://dashboard.reown.com. Passed as a `projectId` query parameter

    on every request.'
  in: query
  name: projectIdAuth
  parameter: projectId
  sources:
  - openapi/reown-openapi.yml
  type: apiKey
slug: reown-authentication
source_filename: reown-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reown-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: projectIdAuth\n  type: apiKey\n  in: query\n  parameter: projectId\n  description: |-\n    Reown project ID from the Reown Dashboard at\n    https://dashboard.reown.com. Passed as a `projectId` query parameter\n    on every request.\n  sources:\n  - openapi/reown-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reown/refs/heads/main/authentication/reown-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Wallets
- WalletConnect
- AppKit
- RPC
---
