---
api_key_in:
- header
api_specs:
- filename: desci-labs-dpid-resolver-openapi.json
  format: json
  label: dPID Resolver API
  slug: dpid-resolver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/desci-labs/refs/heads/main/openapi/desci-labs-dpid-resolver-openapi.json
auth_types:
- none
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Desci Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeSci Labs secures its APIs with none, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DeSci Labs
provider_slug: desci-labs
scheme_count: 4
schemes:
- applies_to: https://beta.dpid.org/api
  name: dpid-resolver-public
  service: dPID Resolver API
  type: none
- docs: https://desci-labs.github.io/nodes/
  in: header
  name: nodes-api-key
  note: API key generated at nodes.desci.com profile; set via nodes-lib setApiKey().
  service: DeSci Nodes backend (desci-server)
  type: apiKey
- name: nodes-signer
  note: Metamask signer or signerFromPkey private-key signer for publishing/on-chain actions.
  service: DeSci Nodes publishing
  type: crypto-signature
- alt: bearer
  docs: https://mcp.sciweave.com
  name: sciweave-mcp-oauth
  service: SciWeave MCP Server
  type: oauth2
slug: desci-labs-authentication
source_filename: desci-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/desci-labs/nodes/blob/develop/nodes-lib/README.md, https://github.com/desci-labs/sciweave-mcp\nsummary:\n  types:\n  - none\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows: []\nnote: >-\n  The public dPID Resolver API (beta.dpid.org) requires no authentication — it is a read-only\n  resolver with no securitySchemes in its OpenAPI. The DeSci Nodes backend (desci-server, via\n  @desci-labs/nodes-lib) authenticates with a per-user API key created under the profile at\n  nodes.desci.com and set via setApiKey; write operations on draft nodes additionally require\n  cryptographic signing (Metamask signer or a private-key signer). The SciWeave MCP server\n  authenticates with OAuth 2.0 or a Bearer API key.\nschemes:\n- name: dpid-resolver-public\n  service: dPID Resolver API\n  type: none\n  applies_to: https://beta.dpid.org/api\n- name: nodes-api-key\n  service: DeSci Nodes backend (desci-server)\n\
  \  type: apiKey\n  in: header\n  docs: https://desci-labs.github.io/nodes/\n  note: API key generated at nodes.desci.com profile; set via nodes-lib setApiKey().\n- name: nodes-signer\n  service: DeSci Nodes publishing\n  type: crypto-signature\n  note: Metamask signer or signerFromPkey private-key signer for publishing/on-chain actions.\n- name: sciweave-mcp-oauth\n  service: SciWeave MCP Server\n  type: oauth2\n  alt: bearer\n  docs: https://mcp.sciweave.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/desci-labs/refs/heads/main/authentication/desci-labs-authentication.yml
summary_line: none/apiKey/oauth2 · 4 schemes
tags:
- Company
- Ai Enterprise Software
- Research Infrastructure
- Decentralized Science
- Scholarly Communication
- Persistent Identifiers
- Open Access
- AI Research Tools
- IPFS
- Model Context Protocol
---
