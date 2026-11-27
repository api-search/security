---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cosvoice-com-activity-api-openapi.yml
  format: yaml
  label: CosVoice Activity API
  slug: cosvoice-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-activity-api-openapi.yml
- filename: cosvoice-com-calls-api-openapi.yml
  format: yaml
  label: CosVoice Calls API
  slug: cosvoice-com-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-calls-api-openapi.yml
- filename: cosvoice-com-contacts-api-openapi.yml
  format: yaml
  label: CosVoice Contacts API
  slug: cosvoice-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-contacts-api-openapi.yml
- filename: cosvoice-com-emails-api-openapi.yml
  format: yaml
  label: CosVoice Emails API
  slug: cosvoice-com-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-emails-api-openapi.yml
- filename: cosvoice-com-history-api-openapi.yml
  format: yaml
  label: CosVoice History API
  slug: cosvoice-com-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-history-api-openapi.yml
- filename: cosvoice-com-line-api-openapi.yml
  format: yaml
  label: CosVoice Line API
  slug: cosvoice-com-line-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-line-api-openapi.yml
- filename: cosvoice-com-messages-api-openapi.yml
  format: yaml
  label: CosVoice Messages API
  slug: cosvoice-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-messages-api-openapi.yml
- filename: cosvoice-com-reservations-api-openapi.yml
  format: yaml
  label: CosVoice Reservations API
  slug: cosvoice-com-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-reservations-api-openapi.yml
- filename: cosvoice-com-settings-api-openapi.yml
  format: yaml
  label: CosVoice Settings API
  slug: cosvoice-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-settings-api-openapi.yml
- filename: cosvoice-com-webhook-api-openapi.yml
  format: yaml
  label: CosVoice Webhook API
  slug: cosvoice-com-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosvoice-com/openapi/cosvoice-com-webhook-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CosVoice Authentication
name_suffix: Authentication
oauth_flows: []
overview: CosVoice secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CosVoice
provider_slug: cosvoice-com
scheme_count: 3
schemes:
- applies_to: REST API https://cosvoice.com/api/v1 and the MCP server https://cosvoice.com/mcp
  description: A line's API key (cv_live_…), from Settings → Connect your agent.
  docs_quote: 'Your key is in Settings → Connect. Send it as Authorization: Bearer cv_live_…'
  key_prefix: cv_live_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cosvoice-com-openapi.yml
  - https://cosvoice.com/docs
  type: http
- applies_to: MCP server https://cosvoice.com/mcp
  description: The remote MCP server at https://cosvoice.com/mcp is connected by URL with OAuth 2.1 (PKCE, dynamic client registration; no key to paste). The user signs in on a CosVoice page and presses Allow; access is revoked in Settings → Connect. Not declared in the OpenAPI, which covers only the REST API.
  dynamic_client_registration: true
  flows:
  - authorizationCode
  name: mcpOAuth
  pkce: true
  sources:
  - https://cosvoice.com/llms-full.txt
  - https://cosvoice.com/docs
  type: oauth2
- applies_to: MCP server
  description: 'If a connector only accepts a plain URL with no sign-in, use https://cosvoice.com/mcp/k/<key> . That URL is a password: keep it out of shared chats, and make a new key if it leaks.'
  in: path
  name: mcpKeyUrl
  sources:
  - https://cosvoice.com/docs
  type: apiKey
slug: cosvoice-com-authentication
source_filename: cosvoice-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cosvoice.com/docs\ndocs: https://cosvoice.com/docs\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A line's API key (cv_live_…), from Settings → Connect your agent.\n  key_prefix: cv_live_\n  applies_to: REST API https://cosvoice.com/api/v1 and the MCP server https://cosvoice.com/mcp\n  docs_quote: \"Your key is in Settings → Connect. Send it as Authorization: Bearer cv_live_…\"\n  sources:\n  - openapi/cosvoice-com-openapi.yml\n  - https://cosvoice.com/docs\n- name: mcpOAuth\n  type: oauth2\n  description: The remote MCP server at https://cosvoice.com/mcp is connected by URL with OAuth 2.1 (PKCE, dynamic client registration; no key to paste). The user signs in on a CosVoice page and presses Allow; access is revoked in Settings → Connect. Not declared in the OpenAPI, which covers only the REST API.\n  applies_to: MCP server https://cosvoice.com/mcp\n\
  \  flows: [authorizationCode]\n  pkce: true\n  dynamic_client_registration: true\n  sources:\n  - https://cosvoice.com/llms-full.txt\n  - https://cosvoice.com/docs\n- name: mcpKeyUrl\n  type: apiKey\n  in: path\n  description: \"If a connector only accepts a plain URL with no sign-in, use https://cosvoice.com/mcp/k/<key> . That URL is a password: keep it out of shared chats, and make a new key if it leaks.\"\n  applies_to: MCP server\n  sources:\n  - https://cosvoice.com/docs\nkey_management: \"API keys are shown once and stored hashed. Replace one any time.\"\n"
source_yaml_url: https://artifacts.apis.io/cosvoice-com/authentication/cosvoice-com-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- AI Agents
- Voice
- Telephony
- Phone Numbers
- AI Receptionist
- Call Transcription
- MCP
- Small Business
---
