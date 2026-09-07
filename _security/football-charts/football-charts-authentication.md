---
anonymous_access: false
api_key_in:
- header
- path
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Football Charts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Football Charts secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Football Charts
provider_slug: football-charts
scheme_count: 4
schemes:
- format: Bearer fc_<key>
  in: header
  name: bearerApiKey
  parameter: Authorization
  sources:
  - https://www.football-charts.com/developers
  - live 401 body
  surfaces:
  - rest
  - mcp-remote
  type: apiKey
- in: header
  name: xApiKey
  note: Not shown on the developer page — discovered in the API's own 401 message, which names both accepted headers.
  parameter: X-API-Key
  sources:
  - live 401 body from https://footballcharts-backend.onrender.com/api/v1/leagues/
  surfaces:
  - rest
  type: apiKey
- format: https://mcp.football-charts.com/<fc_key>/mcp
  in: path
  name: mcpUrlPathKey
  note: Documented for claude.ai custom connectors, whose configuration field accepts only a URL. The provider states keys are read-only and replaceable, so a key in a URL grants published statistics and nothing else.
  parameter: <key>
  sources:
  - https://www.football-charts.com/developers
  surfaces:
  - mcp-remote
  type: apiKey
- in: environment
  name: fcApiKeyEnv
  parameter: FC_API_KEY
  sources:
  - https://github.com/ddevetak/footballcharts-mcp/blob/main/server.json
  surfaces:
  - mcp-stdio
  type: apiKey
slug: football-charts-authentication
source_filename: football-charts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://www.football-charts.com/developers\ndocs: https://www.football-charts.com/developers\nnote: >-\n  DERIVED-FROM-SPEC was not possible — Football Charts publishes no OpenAPI. This profile is read\n  from the provider's developer page, its self-describing API descriptor at\n  https://footballcharts-backend.onrender.com/api/v1/, its open-source MCP server, and live\n  unauthenticated probes of the API (which return the auth instructions in the error body).\nsummary:\n  types: [apiKey]\n  api_key_in: [header, path]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  anonymous_surfaces:\n    - 'GET https://footballcharts-backend.onrender.com/api/v1/ (self-describing descriptor)'\n    - 'POST https://mcp.football-charts.com/mcp — initialize and tools/list'\nschemes:\n  - name: bearerApiKey\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Bearer fc_<key>'\n    surfaces:\
  \ [rest, mcp-remote]\n    sources: ['https://www.football-charts.com/developers', 'live 401 body']\n  - name: xApiKey\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    surfaces: [rest]\n    sources: ['live 401 body from https://footballcharts-backend.onrender.com/api/v1/leagues/']\n    note: >-\n      Not shown on the developer page — discovered in the API's own 401 message, which names both\n      accepted headers.\n  - name: mcpUrlPathKey\n    type: apiKey\n    in: path\n    parameter: '<key>'\n    format: 'https://mcp.football-charts.com/<fc_key>/mcp'\n    surfaces: [mcp-remote]\n    sources: ['https://www.football-charts.com/developers']\n    note: >-\n      Documented for claude.ai custom connectors, whose configuration field accepts only a URL. The\n      provider states keys are read-only and replaceable, so a key in a URL grants published\n      statistics and nothing else.\n  - name: fcApiKeyEnv\n    type: apiKey\n    in: environment\n    parameter: FC_API_KEY\n\
  \    surfaces: [mcp-stdio]\n    sources: ['https://github.com/ddevetak/footballcharts-mcp/blob/main/server.json']\nkey_issuance:\n  self_serve: true\n  endpoint: 'POST https://footballcharts-backend.onrender.com/api/v1/keys/register/'\n  request_body: '{\"email\": \"you@example.com\"}'\n  web_form: https://www.football-charts.com/developers\n  key_prefix: fc_\n  shown_once: true\n  rotation: 'Provider states a new key can be issued at any time; keys are read-only.'\n  cost: free\nx-evidence:\n  - {fetched: '2026-09-04', url: 'https://footballcharts-backend.onrender.com/api/v1/leagues/', http_status: 401, body: '{\"error\": {\"code\": \"missing_key\", \"message\": \"Pass your API key as \\\"Authorization: Bearer fc_...\\\" or \\\"X-API-Key\\\". Free keys: POST /api/v1/keys/register/\"}}'}\n  - {fetched: '2026-09-04', url: 'https://footballcharts-backend.onrender.com/api/v1/leagues/', http_status: 401, sent: 'Authorization: Bearer <invalid>', body: '{\"error\": {\"code\": \"unknown_key\"\
  , \"message\": \"API key not recognised.\"}}'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/football-charts/refs/heads/main/authentication/football-charts-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- football
- soccer
- sports
- sports-data
- statistics
- results
- standings
- fixtures
- predictions
- probability-models
- monte-carlo
- mcp
- agent-native
- free-api
---
