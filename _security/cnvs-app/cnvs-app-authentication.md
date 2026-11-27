---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: cnvs-app-ai-facing-api-openapi.yml
  format: yaml
  label: cnvs.app AI Facing API
  slug: cnvs-app-ai-facing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnvs-app/openapi/cnvs-app-ai-facing-api-openapi.yml
- filename: cnvs-app-boards-api-openapi.yml
  format: yaml
  label: cnvs.app Boards API
  slug: cnvs-app-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnvs-app/openapi/cnvs-app-boards-api-openapi.yml
- filename: cnvs-app-discovery-api-openapi.yml
  format: yaml
  label: cnvs.app Discovery API
  slug: cnvs-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnvs-app/openapi/cnvs-app-discovery-api-openapi.yml
- filename: cnvs-app-items-api-openapi.yml
  format: yaml
  label: cnvs.app Items API
  slug: cnvs-app-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnvs-app/openapi/cnvs-app-items-api-openapi.yml
- filename: cnvs-app-kanban-api-openapi.yml
  format: yaml
  label: cnvs.app Kanban API
  slug: cnvs-app-kanban-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnvs-app/openapi/cnvs-app-kanban-api-openapi.yml
- filename: cnvs-app-reads-api-openapi.yml
  format: yaml
  label: cnvs.app Reads API
  slug: cnvs-app-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnvs-app/openapi/cnvs-app-reads-api-openapi.yml
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: cnvs.app Authentication
name_suffix: Authentication
oauth_flows: []
overview: cnvs.app secures its APIs with none and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: cnvs.app
provider_slug: cnvs-app
scheme_count: 3
schemes:
- description: No credential by default. Anyone who knows the board ID can read and write that board, identical to sharing the browser URL (https://cnvs.app/llms-full.txt).
  name: BoardID
  sources:
  - https://cnvs.app/docs/api/
  - https://cnvs.app/llms-full.txt
  type: none
- description: '8-char [a-z0-9] access key (6-char legacy keys also accepted). Required for write operations on any locked board, and for ALL operations on a board locked with mode=all. Obtain via POST /api/boards/{id}/lock, which returns the key ONCE on first lock. "No recovery: lose the key, lose the board."'
  in: header
  name: BoardKey
  parameter: X-Board-Key
  sources:
  - openapi/cnvs-app-openapi.yml
  - https://cnvs.app/docs/api/
  type: apiKey
- description: Server-to-server infrastructure credential (single shared secret, not issued to the public). A valid token selects the infrastructure REST/MCP and board-create rate tiers; it does not bypass import, validation, per-board, board-access-lock or security limits (https://cnvs.app/quotas.json).
  in: header
  name: ImportToken
  parameter: X-Import-Token
  sources:
  - https://cnvs.app/quotas.json
  - openapi/cnvs-app-openapi.yml
  type: apiKey
slug: cnvs-app-authentication
source_filename: cnvs-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cnvs.app/docs/api/\ndocs: https://cnvs.app/docs/api/\nsummary:\n  types:\n  - none\n  - apiKey\n  api_key_in:\n  - header\n  default: none\n  note: \"Docs: \\\"Auth : none by default — the board ID is the access key. Optional 8-char PIN lock via X-Board-Key header.\\\" There is no account, no API key and no OAuth.\"\nschemes:\n- name: BoardID\n  type: none\n  description: \"No credential by default. Anyone who knows the board ID can read and write that board, identical to sharing the browser URL (https://cnvs.app/llms-full.txt).\"\n  sources:\n  - https://cnvs.app/docs/api/\n  - https://cnvs.app/llms-full.txt\n- name: BoardKey\n  type: apiKey\n  in: header\n  parameter: X-Board-Key\n  description: '8-char [a-z0-9] access key (6-char legacy keys also accepted). Required for write operations on any locked board, and for ALL operations on a board locked with mode=all. Obtain via POST /api/boards/{id}/lock, which returns\
  \ the key ONCE on first lock. \"No recovery: lose the key, lose the board.\"' \n  sources:\n  - openapi/cnvs-app-openapi.yml\n  - https://cnvs.app/docs/api/\n- name: ImportToken\n  type: apiKey\n  in: header\n  parameter: X-Import-Token\n  description: \"Server-to-server infrastructure credential (single shared secret, not issued to the public). A valid token selects the infrastructure REST/MCP and board-create rate tiers; it does not bypass import, validation, per-board, board-access-lock or security limits (https://cnvs.app/quotas.json).\"\n  sources:\n  - https://cnvs.app/quotas.json\n  - openapi/cnvs-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/cnvs-app/authentication/cnvs-app-authentication.yml
summary_line: none/apiKey · 3 schemes
tags:
- Company
- Whiteboard
- Collaboration
- Real-Time
- Kanban
- MCP
- AI Agents
- Diagramming
---
