---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Silmaril Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Silmaril secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Silmaril
provider_slug: silmaril
scheme_count: 2
schemes:
- applies_to: Firewall classify API (SDKs) and LiteLLM guardrail endpoint
  detail: A Silmaril-issued API key is supplied to the Firewall client (SDK apiKey / api_key + tenant classify apiUrl) and passed as the `x-api-key` header when configuring the LiteLLM guardrail (SILMARIL_API_KEY + SILMARIL_GUARDRAIL_URL). Credentials are provisioned by Silmaril; the product is not self-serve yet.
  in: header
  name: FirewallApiKey
  type: apiKey
- applies_to: Silmaril Firewall MCP evidence server (firewall-mcp.silmaril.dev)
  detail: The hosted MCP server uses OAuth via the customer's Auth0 organization with hosted OAuth discovery; the signed-in user's access is forwarded to the read-only evidence API. Access is scope-gated (aggregate/search tools need less access than full payload/trace tools).
  flow: authorizationCode
  name: McpOAuth
  provider: Auth0
  type: oauth2
slug: silmaril-authentication
source_filename: silmaril-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://silmaril.dev/docs\ndocs: https://silmaril.dev/docs\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: FirewallApiKey\n  type: apiKey\n  in: header\n  applies_to: Firewall classify API (SDKs) and LiteLLM guardrail endpoint\n  detail: >-\n    A Silmaril-issued API key is supplied to the Firewall client (SDK apiKey /\n    api_key + tenant classify apiUrl) and passed as the `x-api-key` header when\n    configuring the LiteLLM guardrail (SILMARIL_API_KEY + SILMARIL_GUARDRAIL_URL).\n    Credentials are provisioned by Silmaril; the product is not self-serve yet.\n- name: McpOAuth\n  type: oauth2\n  flow: authorizationCode\n  provider: Auth0\n  applies_to: Silmaril Firewall MCP evidence server (firewall-mcp.silmaril.dev)\n  detail: >-\n    The hosted MCP server uses OAuth via the customer's Auth0 organization with\n    hosted OAuth discovery; the signed-in user's\
  \ access is forwarded to the\n    read-only evidence API. Access is scope-gated (aggregate/search tools need\n    less access than full payload/trace tools).\nnotes: >-\n  No OpenAPI is published, so this profile is searched from the developer docs\n  and the MCP server repo rather than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silmaril/refs/heads/main/authentication/silmaril-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- AI Security
- AI Firewall
- Prompt Injection
- Agent Security
- Runtime Security
- Guardrails
- MCP
- LLM Security
- Developer Tools
---
