---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CreditPolicy.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: CreditPolicy.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CreditPolicy.ai
provider_slug: creditpolicy-ai
scheme_count: 2
schemes:
- applies_to: https://creditpolicy.ai/api/mcp
  description: Sign in with OAuth from Claude, ChatGPT or Perplexity. No keys to paste
  discovery:
    authorization_server: https://txmbawsgucegjjaxcvae.supabase.co/auth/v1
    authorization_server_metadata: https://txmbawsgucegjjaxcvae.supabase.co/auth/v1/.well-known/oauth-authorization-server
    protected_resource_metadata: https://creditpolicy.ai/.well-known/oauth-protected-resource
  dynamic_client_registration: true
  evidence: Authorization server metadata (HTTP 200, fetched 2026-11-04); PRM HTTP 200.
  flows:
  - authorization_code
  - refresh_token
  name: oauth2
  pkce:
  - S256
  - plain
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- applies_to: https://creditpolicy.ai/api/mcp
  description: Personal cpk_ keys for Claude Desktop, Cursor and automation that can't do OAuth
  name: access-key
  note: Header name and placement are not documented on the public page.
  prefix: cpk_
  type: apiKey
slug: creditpolicy-ai-authentication
source_filename: creditpolicy-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://creditpolicy.ai/mcp\ndocs: https://creditpolicy.ai/mcp\nname: CreditPolicy.ai authentication\nnote: No OpenAPI is published; the profile is read from the /mcp documentation page and the published OAuth discovery documents. The /docs path redirects to /login (docs are behind sign-in).\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://creditpolicy.ai/api/mcp\n  description: \"Sign in with OAuth from Claude, ChatGPT or Perplexity. No keys to paste\"\n  discovery:\n    protected_resource_metadata: https://creditpolicy.ai/.well-known/oauth-protected-resource\n    authorization_server: https://txmbawsgucegjjaxcvae.supabase.co/auth/v1\n    authorization_server_metadata: https://txmbawsgucegjjaxcvae.supabase.co/auth/v1/.well-known/oauth-authorization-server\n  flows: [authorization_code, refresh_token]\n  pkce: [S256, plain]\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [client_secret_basic,\
  \ client_secret_post, none]\n  evidence: Authorization server metadata (HTTP 200, fetched 2026-11-04); PRM HTTP 200.\n- name: access-key\n  type: apiKey\n  applies_to: https://creditpolicy.ai/api/mcp\n  prefix: cpk_\n  description: \"Personal cpk_ keys for Claude Desktop, Cursor and automation that can't do OAuth\"\n  note: Header name and placement are not documented on the public page.\n"
source_yaml_url: https://artifacts.apis.io/creditpolicy-ai/authentication/creditpolicy-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Credit Policy
- Lending
- Mortgage Brokers
- MCP
- Financial Services
- Australia
---
