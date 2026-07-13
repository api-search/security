---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Flashbots Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flashbots secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flashbots
provider_slug: flashbots
scheme_count: 1
schemes:
- description: 'Format: <publicKeyAddress>:<EIP-191 signature of keccak256(body)>'
  in: header
  name: flashbotsSignature
  parameter: X-Flashbots-Signature
  sources:
  - openapi/flashbots-openapi.yml
  type: apiKey
slug: flashbots-authentication
source_filename: flashbots-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flashbots-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: flashbotsSignature\n  type: apiKey\n  in: header\n  parameter: X-Flashbots-Signature\n  description: 'Format: <publicKeyAddress>:<EIP-191 signature of keccak256(body)>'\n  sources:\n  - openapi/flashbots-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flashbots/refs/heads/main/authentication/flashbots-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- MEV
- Ethereum
- Blockchain
- JSON-RPC
- Relay
- MEV-Boost
- MEV-Share
- Flashbots Protect
- SUAVE
- Block Builders
- Validators
---
