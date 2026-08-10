---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- none
description: ''
kind: authentication
layout: security
method: probed
name: Andium Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Andium secures its APIs with oauth2, openIdConnect, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Andium
provider_slug: andium
scheme_count: 3
schemes:
- applies_to: https://shop.andium.com/api/ucp/mcp (tools/list, search_catalog, lookup_catalog, get_product)
  name: none
  sources:
  - mcp/andium-mcp-tools.json
  type: none
- description: Every UCP tool call carries meta.ucp-agent.profile — a URI identifying the calling agent. A missing or unresolvable profile returns JSON-RPC error -32001 invalid_profile_url.
  name: ucp-agent-profile
  required: true
  sources:
  - mcp/andium-mcp-tools.json
  type: agentIdentity
- authorizationUrl: https://shopify.com/authentication/85535392078/oauth/authorize
  code_challenge_methods:
  - S256
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/85535392078
  jwks_uri: https://shopify.com/authentication/85535392078/.well-known/jwks.json
  name: shopify-customer-accounts
  openIdConnectUrl: https://shop.andium.com/.well-known/openid-configuration
  response_types:
  - code
  sources:
  - well-known/andium-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/85535392078/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: andium-authentication
source_filename: andium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://shop.andium.com/.well-known/openid-configuration\ndocs: https://shop.andium.com/agents.md\nsummary:\n  types: [oauth2, openIdConnect, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Two distinct auth postures. The UCP/MCP shopping endpoint accepts anonymous tools/list and\n    catalog reads; transacting requires a UCP agent profile URI in meta.ucp-agent.profile and\n    explicit human approval at payment. Customer accounts use Shopify's hosted OIDC provider.\nschemes:\n  - name: none\n    type: none\n    applies_to: https://shop.andium.com/api/ucp/mcp (tools/list, search_catalog, lookup_catalog, get_product)\n    sources: [mcp/andium-mcp-tools.json]\n  - name: ucp-agent-profile\n    type: agentIdentity\n    description: >-\n      Every UCP tool call carries meta.ucp-agent.profile — a URI identifying the calling agent.\n      A missing or unresolvable profile returns JSON-RPC error -32001\
  \ invalid_profile_url.\n    required: true\n    sources: [mcp/andium-mcp-tools.json]\n  - name: shopify-customer-accounts\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/85535392078\n    openIdConnectUrl: https://shop.andium.com/.well-known/openid-configuration\n    authorizationUrl: https://shopify.com/authentication/85535392078/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/85535392078/oauth/token\n    jwks_uri: https://shopify.com/authentication/85535392078/.well-known/jwks.json\n    response_types: [code]\n    code_challenge_methods: [S256]\n    id_token_signing_alg: [RS256]\n    token_endpoint_auth_methods: [client_secret_basic]\n    sources: [well-known/andium-openid-configuration.json]\nx-evidence:\n  - url: https://shop.andium.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://shop.andium.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://shop.andium.com/api/ucp/mcp\n    http_status:\
  \ 200\n    note: tools/list succeeded anonymously\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andium/refs/heads/main/authentication/andium-authentication.yml
summary_line: oauth2/openIdConnect/none · 3 schemes
tags:
- Company
- Energy
- Oil and Gas
- Industrial IoT
- Remote Monitoring
- Methane Detection
- Emissions
- Computer Vision
- Edge Computing
- Commerce
- Model Context Protocol
---
