---
anonymous_access: true
api_key_in: []
api_specs:
- filename: cuqu-net-activities-api-openapi.yml
  format: yaml
  label: CUQU Activities API
  slug: cuqu-net-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuqu-net/openapi/cuqu-net-activities-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CUQU Authentication
name_suffix: Authentication
oauth_flows: []
overview: CUQU secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CUQU
provider_slug: cuqu-net
scheme_count: 2
schemes:
- applies_to: REST GET /api/activity (listActivities) on https://cuqu.net; MCP initialize / tools/list and read-only tools (query_activities, get_activity_card, query_venues, generate_urllink)
  description: The OpenAPI document at cuqu.net/openapi.json declares no securitySchemes; the ai-agent page states initialize/tools/list can be read without a key ("无需密钥即可读取 initialize / tools/list").
  name: anonymous
  type: none
- applies_to: MCP tools/call on https://agent.cuqu.net/mcp, required for write tools create_activity, register_event, create_payment, check_in
  description: 'Personal API key issued on the open platform agent.cuqu.net via WeChat scan login, sent as Authorization: Bearer cq-sk-... The gateway hashes the key (SHA-256) to resolve the user uid and injects it into tool arguments. One active key per user; refreshing revokes the old key. The ai-agent page says write operations need an authorized key with scope restrictions ("需要你授权的 API Key 且有作用域限制"); no scope names are published.'
  issuance: https://agent.cuqu.net/
  key_format: cq-sk- prefix + 32 random hex characters
  name: personalApiKey
  revocation: key refresh invalidates the previous key (open-platform-spec.md)
  scheme: bearer
  type: http
slug: cuqu-net-authentication
source_filename: cuqu-net-authentication.yml
source_heading: Authentication Profile
source_url: https://cuqu.net/llms.txt
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cuqu.net/ai-agent/\ndocs: https://cuqu.net/ai-agent/\nsources:\n- https://cuqu.net/llms.txt\n- https://github.com/cuqu-net/cuqu-skill/blob/main/docs/open-platform-spec.md\nsummary:\n  types:\n  - none\n  - http\nschemes:\n- name: anonymous\n  type: none\n  applies_to: REST GET /api/activity (listActivities) on https://cuqu.net; MCP initialize / tools/list and read-only tools (query_activities, get_activity_card, query_venues, generate_urllink)\n  description: The OpenAPI document at cuqu.net/openapi.json declares no securitySchemes; the ai-agent page states initialize/tools/list can be read without a key (\"无需密钥即可读取 initialize / tools/list\").\n- name: personalApiKey\n  type: http\n  scheme: bearer\n  key_format: cq-sk- prefix + 32 random hex characters\n  applies_to: MCP tools/call on https://agent.cuqu.net/mcp, required for write tools create_activity, register_event, create_payment, check_in\n  description: 'Personal\
  \ API key issued on the open platform agent.cuqu.net via WeChat scan login, sent as Authorization: Bearer cq-sk-... The gateway hashes the key (SHA-256) to resolve the user uid and injects it into tool arguments. One active key per user; refreshing revokes the old key. The ai-agent page says write operations need an authorized key with scope restrictions (\"需要你授权的 API Key 且有作用域限制\"); no scope names are published.'\n  issuance: https://agent.cuqu.net/\n  revocation: key refresh invalidates the previous key (open-platform-spec.md)\nnote: Neither the REST contract nor the MCP gateway uses OAuth; scopes are mentioned but never enumerated, so no scopes/ artifact was written.\n"
source_yaml_url: https://artifacts.apis.io/cuqu-net/authentication/cuqu-net-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Company
- Social
- Event
- Activities
- Community
- Consumer
- MCP
- AI Agents
- China
- WeChat Mini Program
---
