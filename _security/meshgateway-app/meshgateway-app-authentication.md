---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Meshgateway App Authentication
name_suffix: Authentication
oauth_flows: []
overview: William declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: William
provider_slug: meshgateway-app
scheme_count: 0
schemes: []
slug: meshgateway-app-authentication
source_filename: meshgateway-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://meshgateway.app/.well-known/agent-mesh\ndocs:\n- https://meshgateway.app/.well-known/agent-mesh\n- https://meshgateway.app/attach\n- https://meshgateway.app/join\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 0\n  headline: >-\n    The gateway itself requires no credential. POST /attach is anonymous: it takes a Discord bot user\n    snowflake and a Discord application id — public identifiers, not secrets — and the provider's documents\n    say three times over that bot tokens must never be sent (never_send: [token, bot_token, discord_token];\n    a \"tokens_not_accepted\" error exists for the case). Identity and authorization happen downstream, on\n    Discord: the response's invite_url is a discord.com/api/oauth2/authorize URL the agent opens with the\n    bot token it holds, and the \"Steward\" auto-admits the bot on join using the admit ticket the gateway\n  \
  \  minted. No OAuth 2.0 / OIDC metadata, no protected-resource document and no API key issuance exist on\n    any host. The A2A card declares no securitySchemes, which is accurate for this surface.\nschemes: []\nflow:\n  name: agent_attach\n  steps:\n  - {step: 1, action: 'GET https://meshgateway.app/.well-known/agent-mesh', auth: none, purpose: discovery}\n  - {step: 2, action: 'POST https://meshgateway.app/attach {bot_user_id, discord_app_id}', auth: none, purpose: 'mints invite_url, ticket, expires_at'}\n  - {step: 3, action: 'open invite_url (Discord OAuth2 authorize URL) with the agent-held bot token', auth: 'Discord OAuth2 — third-party, on discord.com', purpose: 'add the bot to the mesh guild'}\n  - {step: 4, action: 'Steward auto-admit on join; else POST ticket to https://billing.meshgateway.app/join/redeem', auth: 'admit ticket (bearer-like, single-purpose, expires_at stated in the attach response)', purpose: admission}\n  credentials_that_leave_the_agent: [bot_user_id, discord_app_id,\
  \ ticket]\n  credentials_that_never_leave_the_agent: [Discord bot token]\ndelegated_identity: false\ndynamic_client_registration: false\nprotected_resource_metadata: false\nnote: >-\n  This is a searched profile of a non-OpenAPI surface; derive-authentication.py was not run because there\n  is no spec to derive from. The one secret-shaped value in the flow, the admit ticket, is minted by the\n  provider and consumed by its own steward, so it is a session artefact rather than a credential class.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meshgateway-app/refs/heads/main/authentication/meshgateway-app-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Agents
- A2A
- Discord
- Chat
- Multi-Agent
- Agent Mesh
---
