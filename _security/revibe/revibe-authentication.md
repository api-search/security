---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Revibe Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Revibe secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Revibe
provider_slug: revibe
scheme_count: 2
schemes:
- authorization_endpoint: https://shopify.com/authentication/69517377855/oauth/authorize
  issuer: https://shopify.com/authentication/69517377855
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://revibe.me/.well-known/openid-configuration
  sources:
  - well-known/revibe-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/69517377855/oauth/token
  type: openIdConnect
- description: Universal Commerce Protocol agent-profile handshake required before the hosted MCP endpoint (https://revibe.me/api/ucp/mcp) will return tools; checkout completion additionally requires contemporaneous human buyer approval.
  name: ucp-agent-profile
  sources:
  - well-known/revibe-ucp.json
  - llms/revibe-llms.txt
  type: oauth2
slug: revibe-authentication
source_filename: revibe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://revibe.me/.well-known/openid-configuration\nnotes: >-\n  No developer API with its own OpenAPI/securitySchemes is published. Auth surfaces\n  captured here are (1) the Shopify Customer Account OpenID Connect discovery document\n  served at the storefront, and (2) the UCP agent-profile handshake gating the hosted\n  MCP commerce endpoint (mcp/revibe-mcp.yml). Derived from live discovery docs, not a spec.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://revibe.me/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/69517377855\n  authorization_endpoint: https://shopify.com/authentication/69517377855/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/69517377855/oauth/token\n  sources: [well-known/revibe-openid-configuration.json]\n- name: ucp-agent-profile\n\
  \  type: oauth2\n  description: >-\n    Universal Commerce Protocol agent-profile handshake required before the hosted\n    MCP endpoint (https://revibe.me/api/ucp/mcp) will return tools; checkout completion\n    additionally requires contemporaneous human buyer approval.\n  sources: [well-known/revibe-ucp.json, llms/revibe-llms.txt]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revibe/refs/heads/main/authentication/revibe-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Marketplace
- E-Commerce
- Refurbished Electronics
- Consumer Electronics
- Retail
- UAE
- Agentic Commerce
---
