---
api_key_in:
- config-file
- npmrc
auth_types:
- token
- oauth-browser-login
description: ''
kind: authentication
layout: security
method: searched
name: Bit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bit secures its APIs with token and oauth-browser-login across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bit
provider_slug: bit
scheme_count: 2
schemes:
- applies_to:
  - CLI
  - GraphQL API
  mechanism: bit login (browser-based auth) -> local Bit Cloud auth token
  name: BitCloudToken
  type: token
- applies_to:
  - Bit Cloud npm registry (node.bit.cloud)
  file: .npmrc
  in: file
  mechanism: bit npmrc generate
  name: RegistryToken
  type: apiKey
slug: bit-authentication
source_filename: bit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://bit.dev/reference/reference/using-bvm/\ndocs: https://bit.dev/docs/\nnote: >-\n  Bit has no captured OpenAPI, so this profile is hand-searched from the docs\n  rather than derived. Bit Cloud authentication is token-based: `bit login`\n  performs an interactive OAuth-style browser login and stores a Bit Cloud\n  auth token locally; the token authenticates CLI operations (export, import,\n  ripple CI) and the GraphQL API. For package installation from the Bit Cloud\n  npm registry, `bit npmrc generate` writes registry auth into `.npmrc`.\nsummary:\n  types: [token, oauth-browser-login]\n  api_key_in: [config-file, npmrc]\n  oauth2_flows: []\nschemes:\n- name: BitCloudToken\n  type: token\n  mechanism: \"bit login (browser-based auth) -> local Bit Cloud auth token\"\n  applies_to: [CLI, GraphQL API]\n- name: RegistryToken\n  type: apiKey\n  in: file\n  file: .npmrc\n  mechanism: \"bit npmrc generate\"\n  applies_to: [Bit\
  \ Cloud npm registry (node.bit.cloud)]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bit/refs/heads/main/authentication/bit-authentication.yml
summary_line: token/oauth-browser-login · 2 schemes
tags:
- Company
- Devops
- Component Development
- Frontend
- Monorepo
- npm
- GraphQL
- CLI
- MCP
- Developer Tools
- AI Agents
---
