---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dialnexa-agents-api-openapi.yml
  format: yaml
  label: DialNexa Agents API
  slug: dialnexa-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-agents-api-openapi.yml
- filename: dialnexa-batch-calls-api-openapi.yml
  format: yaml
  label: DialNexa Batch Calls API
  slug: dialnexa-batch-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-batch-calls-api-openapi.yml
- filename: dialnexa-calls-api-openapi.yml
  format: yaml
  label: DialNexa Calls API
  slug: dialnexa-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-calls-api-openapi.yml
- filename: dialnexa-knowledge-base-api-openapi.yml
  format: yaml
  label: DialNexa Knowledge Base API
  slug: dialnexa-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-knowledge-base-api-openapi.yml
- filename: dialnexa-languages-api-openapi.yml
  format: yaml
  label: DialNexa Languages API
  slug: dialnexa-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-languages-api-openapi.yml
- filename: dialnexa-llms-api-openapi.yml
  format: yaml
  label: DialNexa LL Ms API
  slug: dialnexa-llms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-llms-api-openapi.yml
- filename: dialnexa-organization-folders-api-openapi.yml
  format: yaml
  label: DialNexa Organization Folders API
  slug: dialnexa-organization-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-organization-folders-api-openapi.yml
- filename: dialnexa-phone-numbers-api-openapi.yml
  format: yaml
  label: DialNexa Phone Numbers API
  slug: dialnexa-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-phone-numbers-api-openapi.yml
- filename: dialnexa-transcribers-api-openapi.yml
  format: yaml
  label: DialNexa Transcribers API
  slug: dialnexa-transcribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-transcribers-api-openapi.yml
- filename: dialnexa-voices-api-openapi.yml
  format: yaml
  label: DialNexa Voices API
  slug: dialnexa-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-voices-api-openapi.yml
- filename: dialnexa-webhooks-api-openapi.yml
  format: yaml
  label: DialNexa Webhooks API
  slug: dialnexa-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-webhooks-api-openapi.yml
- filename: dialnexa-workflow-leads-api-openapi.yml
  format: yaml
  label: DialNexa Workflow Leads API
  slug: dialnexa-workflow-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-workflow-leads-api-openapi.yml
- filename: dialnexa-workflows-api-openapi.yml
  format: yaml
  label: DialNexa Workflows API
  slug: dialnexa-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dialnexa Authentication
name_suffix: Authentication
oauth_flows: []
overview: DialNexa secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DialNexa
provider_slug: dialnexa
scheme_count: 2
schemes:
- description: Workspace API key sent as the Bearer token on every request. The key is a key_id:secret pair (two segments separated by a colon) created in Dashboard -> Settings -> API Keys and shown once; send the FULL value, not just the key id. One key per environment is recommended. 401 {statusCode, message, error} on missing/revoked/malformed keys. Do not use x-api-key for v1 endpoints.
  name: bearer
  scheme: bearer
  sources:
  - openapi/dialnexa-agents-api-openapi.yml
  - openapi/dialnexa-batch-calls-api-openapi.yml
  - openapi/dialnexa-calls-api-openapi.yml
  - openapi/dialnexa-knowledge-base-api-openapi.yml
  - openapi/dialnexa-languages-api-openapi.yml
  - openapi/dialnexa-llms-api-openapi.yml
  - openapi/dialnexa-organization-folders-api-openapi.yml
  - openapi/dialnexa-phone-numbers-api-openapi.yml
  - openapi/dialnexa-transcribers-api-openapi.yml
  - openapi/dialnexa-voices-api-openapi.yml
  - openapi/dialnexa-webhooks-api-openapi.yml
  - openapi/dialnexa-workflow-leads-api-openapi.yml
  - openapi/dialnexa-workflows-api-openapi.yml
  type: http
- applies_to: https://api.dialnexa.com/v1/mcp (MCP surface only; REST issues no public OAuth tokens)
  authorization_server: https://api.dialnexa.com
  metadata: well-known/dialnexa-api-oauth-authorization-server.json
  name: mcp-oauth
  scheme: oauth2.1 authorization-code + PKCE
  scopes:
  - mcp:read
  - mcp:write
  - offline_access
  - openid
  sources:
  - https://dialnexa.com/docs/mcp-tools/overview.md
  - https://api.dialnexa.com/.well-known/oauth-authorization-server
  type: oauth2
slug: dialnexa-authentication
source_filename: dialnexa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://dialnexa.com/docs/api-reference/authentication.md + OpenAPI securitySchemes (13 refined specs)\nsummary:\n  types:\n  - http\n  styles:\n  - bearer-api-key (REST)\n  - oauth2.1 (MCP)\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dialnexa-agents-api-openapi.yml\n  - openapi/dialnexa-batch-calls-api-openapi.yml\n  - openapi/dialnexa-calls-api-openapi.yml\n  - openapi/dialnexa-knowledge-base-api-openapi.yml\n  - openapi/dialnexa-languages-api-openapi.yml\n  - openapi/dialnexa-llms-api-openapi.yml\n  - openapi/dialnexa-organization-folders-api-openapi.yml\n  - openapi/dialnexa-phone-numbers-api-openapi.yml\n  - openapi/dialnexa-transcribers-api-openapi.yml\n  - openapi/dialnexa-voices-api-openapi.yml\n  - openapi/dialnexa-webhooks-api-openapi.yml\n  - openapi/dialnexa-workflow-leads-api-openapi.yml\n  - openapi/dialnexa-workflows-api-openapi.yml\n  description: Workspace API key sent\
  \ as the Bearer token on every request. The key is a key_id:secret pair (two\n    segments separated by a colon) created in Dashboard -> Settings -> API Keys and shown once; send the FULL value,\n    not just the key id. One key per environment is recommended. 401 {statusCode, message, error} on missing/revoked/malformed\n    keys. Do not use x-api-key for v1 endpoints.\n- name: mcp-oauth\n  type: oauth2\n  scheme: oauth2.1 authorization-code + PKCE\n  applies_to: https://api.dialnexa.com/v1/mcp (MCP surface only; REST issues no public OAuth tokens)\n  authorization_server: https://api.dialnexa.com\n  metadata: well-known/dialnexa-api-oauth-authorization-server.json\n  scopes:\n  - mcp:read\n  - mcp:write\n  - offline_access\n  - openid\n  sources:\n  - https://dialnexa.com/docs/mcp-tools/overview.md\n  - https://api.dialnexa.com/.well-known/oauth-authorization-server\ndocs: https://dialnexa.com/docs/api-reference/authentication\nagent_provisioning:\n  note: 'DialNexa publishes machine-readable\
  \ key-provisioning guidance for AI agents: an auth.md addressed to agents\n    (authentication/dialnexa-auth.md, from https://dialnexa.com/auth.md) and an agent_auth block in https://dialnexa.com/.well-known/oauth-authorization-server\n    naming identity type account_api_key, credential type api_key_bearer, and step-by-step registration instructions.'\nwebhook_signing:\n  header: x-dialnexa-signature\n  algorithm: HMAC-SHA256 hex over raw body\n  detail: asyncapi/dialnexa-webhooks.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/authentication/dialnexa-authentication.yml
summary_line: http · 2 schemes
tags:
- Voice AI
- AI Agents
- Telephony
- Lead Qualification
- Multilingual
---
