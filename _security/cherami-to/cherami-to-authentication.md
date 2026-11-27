---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cherami-to-access-api-openapi.yml
  format: yaml
  label: Cherami Access API
  slug: cherami-to-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-access-api-openapi.yml
- filename: cherami-to-drafts-api-openapi.yml
  format: yaml
  label: Cherami Drafts API
  slug: cherami-to-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-drafts-api-openapi.yml
- filename: cherami-to-feedback-api-openapi.yml
  format: yaml
  label: Cherami Feedback API
  slug: cherami-to-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-feedback-api-openapi.yml
- filename: cherami-to-inboxes-api-openapi.yml
  format: yaml
  label: Cherami Inboxes API
  slug: cherami-to-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-inboxes-api-openapi.yml
- filename: cherami-to-labels-api-openapi.yml
  format: yaml
  label: Cherami Labels API
  slug: cherami-to-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-labels-api-openapi.yml
- filename: cherami-to-messages-api-openapi.yml
  format: yaml
  label: Cherami Messages API
  slug: cherami-to-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-messages-api-openapi.yml
- filename: cherami-to-sending-api-openapi.yml
  format: yaml
  label: Cherami Sending API
  slug: cherami-to-sending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-sending-api-openapi.yml
- filename: cherami-to-threads-api-openapi.yml
  format: yaml
  label: Cherami Threads API
  slug: cherami-to-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-threads-api-openapi.yml
- filename: cherami-to-trash-api-openapi.yml
  format: yaml
  label: Cherami Trash API
  slug: cherami-to-trash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-trash-api-openapi.yml
- filename: cherami-to-webhooks-api-openapi.yml
  format: yaml
  label: Cherami Webhooks API
  slug: cherami-to-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cherami Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cherami secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cherami
provider_slug: cherami-to
scheme_count: 2
schemes:
- bearerFormat: Cherami API key
  description: Cherami API key (ch_...), from Account → API keys or from redeeming a human-approved phrase. Every key reaches all of the account's inboxes and mail. MCP OAuth tokens and browser sessions are not accepted.
  how_to_obtain: Sign in at Account → API keys and choose Create API key (shown only once), or, for an agent, redeem a human-approved phrase (redeemClaim) whose 201 returns the key as `credential` with token_type Bearer.
  key_prefix: ch_
  name: apiKey
  scheme: bearer
  sources:
  - openapi/cherami-to-openapi.yml
  - https://cherami.to/docs/quickstart
  surface: HTTP API (https://cherami.to/v1)
  type: http
- description: Remote MCP with OAuth (CIMD or DCR); OAuth mail scope cherami_mail:full. The MCP server also accepts a Cherami API key in the Authorization header when a client cannot complete OAuth.
  name: mcpOAuth
  scopes:
  - cherami_mail:full
  sources:
  - https://cherami.to/docs/mcp
  surface: Hosted MCP server (https://cherami.to/mcp)
  type: oauth2
slug: cherami-to-authentication
source_filename: cherami-to-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://cherami.to/docs/quickstart\ndocs: https://cherami.to/docs/quickstart\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: Cherami API key\n  surface: HTTP API (https://cherami.to/v1)\n  description: Cherami API key (ch_...), from Account → API keys or from redeeming a human-approved phrase. Every\n    key reaches all of the account's inboxes and mail. MCP OAuth tokens and browser sessions are not accepted.\n  key_prefix: ch_\n  how_to_obtain: Sign in at Account → API keys and choose Create API key (shown only once), or, for an agent, redeem\n    a human-approved phrase (redeemClaim) whose 201 returns the key as `credential` with token_type Bearer.\n  sources:\n  - openapi/cherami-to-openapi.yml\n  - https://cherami.to/docs/quickstart\n- name: mcpOAuth\n  type: oauth2\n  surface: Hosted MCP server (https://cherami.to/mcp)\n  description: Remote MCP with\
  \ OAuth (CIMD or DCR); OAuth mail scope cherami_mail:full. The MCP server also accepts\n    a Cherami API key in the Authorization header when a client cannot complete OAuth.\n  scopes:\n  - cherami_mail:full\n  sources:\n  - https://cherami.to/docs/mcp\ndocs_mcp: https://cherami.to/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/cherami-to/authentication/cherami-to-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Email
- AI Agents
- MCP
- Webhook
- Messaging
- Email API
---
