---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kifly-ai-openapi-generated.yml
  format: yaml
  label: Kifly API
  slug: kifly-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kifly-ai/openapi/_ae-authored/kifly-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Kifly MCP endpoint
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Kifly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kifly declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Kifly
provider_slug: kifly-ai
scheme_count: 4
schemes:
- evidence: 'Authorization: Bearer kfa_live_xxxxxxxxxxxxxxxx'
  header: Authorization
  location: header
  name: Seller API key
  type: http-bearer
- evidence: 'Authorization: Bearer kfn_live_xxxxxxxxxxxxxxxx'
  header: Authorization
  location: header
  name: Network key
  type: http-bearer
- evidence: Discovery at https://kifly.ai/.well-known/oauth-authorization-server , with dynamic client registration at https://kifly.ai/oauth/register . No Kifly seller account needed to register a client. PKCE S256 required.
  how_to_obtain: Use the discovery URL https://kifly.ai/.well-known/oauth-authorization-server and register a client at https://kifly.ai/oauth/register
  name: OAuth 2.1
  type: oauth2
- evidence: 'Send your agent''s UCP profile URL in meta : { "meta": { "ucp-agent": { "profile": "https://your-agent.example/.well-known/ucp" } } }'
  location: body
  name: No credential (UCP profile)
  type: other
slug: kifly-ai-authentication
source_filename: kifly-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://kifly.ai/docs/mcp
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kifly.ai/docs/mcp\nsources:\n- https://kifly.ai/docs/mcp\n- https://kifly.ai/docs/seller-onboarding\ndescription: Authentication methods for Kifly MCP endpoint\nschemes:\n- type: http-bearer\n  name: Seller API key\n  evidence: 'Authorization: Bearer kfa_live_xxxxxxxxxxxxxxxx'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: Network key\n  evidence: 'Authorization: Bearer kfn_live_xxxxxxxxxxxxxxxx'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Discovery at https://kifly.ai/.well-known/oauth-authorization-server , with dynamic client registration at https://kifly.ai/oauth/register\n    . No Kifly seller account needed to register a client. PKCE S256 required.\n  how_to_obtain: Use the discovery URL https://kifly.ai/.well-known/oauth-authorization-server and register a client at https://kifly.ai/oauth/register\n\
  - type: other\n  name: No credential (UCP profile)\n  evidence: 'Send your agent''s UCP profile URL in meta : { \"meta\": { \"ucp-agent\": { \"profile\": \"https://your-agent.example/.well-known/ucp\" }\n    } }'\n  location: body\ndocs: https://kifly.ai/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/kifly-ai/authentication/kifly-ai-authentication.yml
summary_line: 4 schemes
tags:
- AI Commerce
- Catalog Integration
- Shopify
- WooCommerce
- Agent Checkout
- Payments
- AI Agents
---
