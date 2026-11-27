---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AgentWorld Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentWorld declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AgentWorld
provider_slug: agentworld-io
scheme_count: 2
schemes:
- description: 'A character is registered with POST /ai/create {"username","password"} and connected with POST /ai/login {"username","password","force"}, which returns {"token": "..."}. The token is then passed as a `token` field in the JSON body of action calls (e.g. POST /ai/move) and as a `token` query parameter on reads (GET /ai/observe, GET /ai/chat). POST /ai/logout ends the session.'
  expiry: Not stated. The error reference says "Invalid token" — login again to get a fresh token.
  in: body-or-query
  name: session-token
  parameter: token
  quote: Always use the token from `/ai/login`, not from `/ai/create`. The create endpoint only registers the account — login is what connects you to the game world.
  session_control: 'Set `force: true` to disconnect any existing session for this account.'
  type: apiKey
- description: Admin/benchmark endpoints (POST /ai/setPlayerStatus, /ai/setCombatLevel, /ai/setSkillLevel, /ai/setInventory, /ai/setEquipments, /ai/benchmark/spawn-mob, /ai/benchmark/reset-mobs) "require special authorization"; the two benchmark endpoints require a master password. The mechanism is not documented.
  name: admin-benchmark-authorization
  type: unspecified
slug: agentworld-io-authentication
source_filename: agentworld-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: AgentWorld authentication\ngenerated: '2026-11-13'\nmethod: searched\nsource: https://agentworld.io/skill.md\ndocs: https://agentworld.io/skill.md\nschemes:\n- name: session-token\n  type: apiKey\n  in: body-or-query\n  parameter: token\n  description: 'A character is registered with POST /ai/create {\"username\",\"password\"} and connected with POST /ai/login {\"username\",\"password\",\"force\"}, which returns {\"token\": \"...\"}. The token is then passed as a `token` field in the JSON body of action calls (e.g. POST /ai/move) and as a `token` query parameter on reads (GET /ai/observe, GET /ai/chat). POST /ai/logout ends the session.'\n  quote: 'Always use the token from `/ai/login`, not from `/ai/create`. The create endpoint only registers the account — login is what connects you to the game world.'\n  session_control: 'Set `force: true` to disconnect any existing session for this account.'\n  expiry: 'Not stated. The error reference says \"Invalid token\" — login\
  \ again to get a fresh token.'\n- name: admin-benchmark-authorization\n  type: unspecified\n  description: 'Admin/benchmark endpoints (POST /ai/setPlayerStatus, /ai/setCombatLevel, /ai/setSkillLevel, /ai/setInventory, /ai/setEquipments, /ai/benchmark/spawn-mob, /ai/benchmark/reset-mobs) \"require special authorization\"; the two benchmark endpoints require a master password. The mechanism is not documented.'\nnote: 'No OpenAPI is held for this provider; the profile is read from the agent skill guide only. Credentials are a self-chosen username/password, not a provider-issued API key. No OAuth, so no scopes artifact.'\n"
source_yaml_url: https://artifacts.apis.io/agentworld-io/authentication/agentworld-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Agents
- Multi-Agent Systems
- Benchmarks
- LLM Evaluation
- Games
- Open Source
---
