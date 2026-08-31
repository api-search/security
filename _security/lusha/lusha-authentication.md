---
api_key_in:
- header
api_specs:
- filename: lusha-search-api-openapi.yml
  format: yaml
  label: Lusha Search API
  slug: lusha-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-search-api-openapi.yml
- filename: lusha-enrich-api-openapi.yml
  format: yaml
  label: Lusha Enrich API
  slug: lusha-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-enrich-api-openapi.yml
- filename: lusha-search-enrich-api-openapi.yml
  format: yaml
  label: Lusha Search & Enrich API
  slug: lusha-search-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-search-enrich-api-openapi.yml
- filename: lusha-prospecting-api-openapi.yml
  format: yaml
  label: Lusha Prospecting API
  slug: lusha-prospecting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-prospecting-api-openapi.yml
- filename: lusha-lookalikes-api-openapi.yml
  format: yaml
  label: Lusha Lookalikes API
  slug: lusha-lookalike-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-lookalikes-api-openapi.yml
- filename: lusha-buying-group-api-openapi.yml
  format: yaml
  label: Lusha Buying Group API
  slug: lusha-buying-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-buying-group-api-openapi.yml
- filename: lusha-signals-api-openapi.yml
  format: yaml
  label: Lusha Signals API
  slug: lusha-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-signals-api-openapi.yml
- filename: lusha-website-visits-api-openapi.yml
  format: yaml
  label: Lusha Website Visitors API
  slug: lusha-website-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-website-visits-api-openapi.yml
- filename: lusha-filters-api-openapi.yml
  format: yaml
  label: Lusha Filters API
  slug: lusha-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-filters-api-openapi.yml
- filename: lusha-contacts-tables-api-openapi.yml
  format: yaml
  label: Lusha Contacts Tables API
  slug: lusha-contacts-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-contacts-tables-api-openapi.yml
- filename: lusha-companies-tables-api-openapi.yml
  format: yaml
  label: Lusha Companies Tables API
  slug: lusha-companies-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-companies-tables-api-openapi.yml
- filename: lusha-webhooks-api-openapi.yml
  format: yaml
  label: Lusha Webhooks API
  slug: lusha-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-webhooks-api-openapi.yml
- filename: lusha-account-api-openapi.yml
  format: yaml
  label: Lusha Account API
  slug: lusha-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-account-api-openapi.yml
- filename: lusha-account-management-api-openapi.yml
  format: yaml
  label: Lusha Account Management API
  slug: lusha-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-account-management-api-openapi.yml
- filename: lusha-company-filters-api-openapi.yml
  format: yaml
  label: Lusha Company Filters API
  slug: lusha-company-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-company-filters-api-openapi.yml
- filename: lusha-contact-filters-api-openapi.yml
  format: yaml
  label: Lusha Contact Filters API
  slug: lusha-contact-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-contact-filters-api-openapi.yml
- filename: lusha-enrichment-api-openapi.yml
  format: yaml
  label: Lusha Enrichment API
  slug: lusha-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-enrichment-api-openapi.yml
- filename: lusha-prospecting-search-enrich-api-openapi.yml
  format: yaml
  label: Lusha Prospecting - Search & Enrich API
  slug: lusha-prospecting-search-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-prospecting-search-enrich-api-openapi.yml
auth_types:
- apiKey
description: 'One credential type on the REST API: a Lusha API key issued in the dashboard and sent in the `api_key` request header on every call. No OAuth, no bearer tokens, no signing, no mTLS. API key issuance is itself plan-gated — the docs restrict keys to Scale-plan users or an active Scale trial. The agent surface is different: the hosted MCP server accepts either an OAuth 2.1 authorization code (scope `mcp`) or the same API key in a lowercase `x-api-key` header.'
kind: authentication
layout: security
method: searched
name: Lusha Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lusha secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lusha
provider_slug: lusha
scheme_count: 3
schemes:
- applies_to: https://api.lusha.com (all 58 v3 operations)
  description: 'Your Lusha API key. You can find this in your Lusha dashboard under API settings.

    Include this key in the `api_key` header for all requests.'
  in: header
  issuance: https://dashboard.lusha.com/api/manage-api-keys
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/lusha-account-api-openapi.yml
  - openapi/lusha-buying-group-api-openapi.yml
  - openapi/lusha-companies-tables-api-openapi.yml
  - openapi/lusha-contacts-tables-api-openapi.yml
  - openapi/lusha-enrich-api-openapi.yml
  - openapi/lusha-filters-api-openapi.yml
  - openapi/lusha-lookalikes-api-openapi.yml
  - openapi/lusha-prospecting-api-openapi.yml
  - openapi/lusha-search-api-openapi.yml
  - openapi/lusha-search-enrich-api-openapi.yml
  - openapi/lusha-signals-api-openapi.yml
  - openapi/lusha-webhooks-api-openapi.yml
  - openapi/lusha-website-visits-api-openapi.yml
  type: apiKey
- applies_to: https://mcp.lusha.com
  description: 'Same Lusha API key, different header name, for MCP clients that do not do OAuth (VS Code, Cursor, n8n, Gemini CLI). The provider documents that the header must be lowercase `x-api-key` and that `Authorization: Bearer` fails.'
  in: header
  name: LushaMCPApiKey
  parameter: x-api-key
  sources:
  - https://docs.lusha.com/mcp-docs
  type: apiKey
- applies_to: https://mcp.lusha.com
  authorization_server: https://auth.lusha.com
  flows:
  - authorizationUrl: https://auth.lusha.com/oauth-ui/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    pkce: S256
    scopes:
    - mcp
    tokenUrl: https://auth.lusha.com/oauth/token
  name: LushaMCPOAuth
  sources:
  - well-known/lusha-oauth-authorization-server.json
  - well-known/lusha-oauth-protected-resource.json
  type: oauth2
  used_by:
  - Claude connector
  - ChatGPT app
  - Codex plugin
slug: lusha-authentication
source_filename: lusha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/lusha-*-api-openapi.yml\ndocs: https://docs.lusha.com/apis/openapi/section/authentication\ndescription: >-\n  One credential type on the REST API: a Lusha API key issued in the dashboard\n  and sent in the `api_key` request header on every call. No OAuth, no bearer\n  tokens, no signing, no mTLS. API key issuance is itself plan-gated — the docs\n  restrict keys to Scale-plan users or an active Scale trial. The agent surface\n  is different: the hosted MCP server accepts either an OAuth 2.1 authorization\n  code (scope `mcp`) or the same API key in a lowercase `x-api-key` header.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  oauth2_scope: mcp\n  oauth2_applies_to: mcp.lusha.com only\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: |-\n    Your Lusha API key. You can find this in your Lusha dashboard under API settings.\n\
  \    Include this key in the `api_key` header for all requests.\n  issuance: https://dashboard.lusha.com/api/manage-api-keys\n  applies_to: https://api.lusha.com (all 58 v3 operations)\n  sources:\n  - openapi/lusha-account-api-openapi.yml\n  - openapi/lusha-buying-group-api-openapi.yml\n  - openapi/lusha-companies-tables-api-openapi.yml\n  - openapi/lusha-contacts-tables-api-openapi.yml\n  - openapi/lusha-enrich-api-openapi.yml\n  - openapi/lusha-filters-api-openapi.yml\n  - openapi/lusha-lookalikes-api-openapi.yml\n  - openapi/lusha-prospecting-api-openapi.yml\n  - openapi/lusha-search-api-openapi.yml\n  - openapi/lusha-search-enrich-api-openapi.yml\n  - openapi/lusha-signals-api-openapi.yml\n  - openapi/lusha-webhooks-api-openapi.yml\n  - openapi/lusha-website-visits-api-openapi.yml\n- name: LushaMCPApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  applies_to: https://mcp.lusha.com\n  description: >-\n    Same Lusha API key, different header name, for MCP clients that\
  \ do not do\n    OAuth (VS Code, Cursor, n8n, Gemini CLI). The provider documents that the\n    header must be lowercase `x-api-key` and that `Authorization: Bearer` fails.\n  sources: [https://docs.lusha.com/mcp-docs]\n- name: LushaMCPOAuth\n  type: oauth2\n  applies_to: https://mcp.lusha.com\n  authorization_server: https://auth.lusha.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.lusha.com/oauth-ui/authorize\n    tokenUrl: https://auth.lusha.com/oauth/token\n    scopes: [mcp]\n    pkce: S256\n    dynamic_client_registration: true\n  used_by: [Claude connector, ChatGPT app, Codex plugin]\n  sources:\n  - well-known/lusha-oauth-authorization-server.json\n  - well-known/lusha-oauth-protected-resource.json\nkey_handling_guidance:\n- Server-side environments only; the docs say not to embed the key client-side.\n- Store in an OS keychain, secrets manager or environment variable, not in shared config files.\n- Rotate keys periodically and remove unused MCP connectors.\n\
  defects:\n- issue: >-\n    The help-centre 401 article instructs callers to send\n    `Authorization: Bearer YOUR_API_KEY`, which contradicts both the API\n    reference and the OpenAPI securityScheme (apiKey, in header, name `api_key`).\n    An agent that follows the help centre will get 401 on every call.\n  url: https://docs.lusha.com/user-guide/lushas-api/lusha-api-error-codes-reference\n  authoritative: openapi securityScheme ApiKeyAuth (api_key header)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/authentication/lusha-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Sales Intelligence
- B2B
- Enrichment
- Contact Data
- Prospecting
- Intent
- Signals
- Lookalikes
- Webhook
- MCP
---
