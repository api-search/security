---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nolimitnodes Authentication
name_suffix: Authentication
oauth_flows: []
overview: NoLimitNodes declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NoLimitNodes
provider_slug: nolimitnodes
scheme_count: 1
schemes:
- evidence: Secure your API requests with API key authentication.
  header: x-api-key
  how_to_obtain: 1 Open the dashboard Sign in at app.nolimitnodes.com . 2 Create or open a project Add a Solana node if the project has no node. 3 Copy the node page and copy its API key. 4 Store the key in a secret manager or environment variable.
  location: header
  name: API Key
  type: apiKey
slug: nolimitnodes-authentication
source_filename: nolimitnodes-authentication.yml
source_heading: Authentication Profile
source_url: https://nolimitnodes.com/docs/authentication
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nolimitnodes.com/docs/authentication\nsources:\n- https://nolimitnodes.com/docs/authentication\n- https://nolimitnodes.com/docs/guides/websocket-authentication\n- https://nolimitnodes.com/docs/api-reference/program-streams/authentication-policy\n- https://nolimitnodes.com/docs/api-reference/solana-rpc/tokens\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Secure your API requests with API key authentication.\n  location: header\n  header: x-api-key\n  how_to_obtain: 1 Open the dashboard Sign in at app.nolimitnodes.com . 2 Create or open a project Add a Solana node if the project has no node.\n    3 Copy the node page and copy its API key. 4 Store the key in a secret manager or environment variable.\ndocs: https://nolimitnodes.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nolimitnodes/refs/heads/main/authentication/nolimitnodes-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Solana
- RPC
- Data-Streams
- MEV
- Infrastructure
---
