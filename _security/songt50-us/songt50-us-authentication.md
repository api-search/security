---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Songt50 Us Authentication
name_suffix: Authentication
oauth_flows: []
overview: sapjilcoding declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: sapjilcoding
provider_slug: songt50-us
scheme_count: 0
schemes: []
slug: songt50-us-authentication
source_filename: songt50-us-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live JSON-RPC probes of both A2A hosts plus the agent cards, server.json/server.py/README of the four MCP repositories\ndocs:\n- https://github.com/SongT-50/korean-public-data-mcp#readme\n- https://github.com/SongT-50/korean-news-mcp#readme\nsummary: >-\n  Every surface sapjilcoding publishes is anonymous. The two A2A agent cards declare no securitySchemes and no\n  security requirements, and their JSON-RPC endpoints answered unauthenticated POSTs on 2026-09-19. The MCP\n  servers document \"no API key required\" for the news server and, for the data servers, hold the upstream\n  data.go.kr and Bank of Korea ECOS keys server-side on the hosted deployment (\"the remote server's API keys are\n  configured on the server; you need your own keys only for a local install\"); no MCP-level credential, OAuth\n  authorization server, protected-resource metadata or dynamic client registration exists. There is no signup,\n  no developer\
  \ portal and no key issuance of any kind.\nschemes: []\nscheme_count: 0\nsurfaces:\n- surface: A2A agents (publicdata-agent.songt50.us, news-agent.songt50.us)\n  auth: none\n  evidence: cards carry no securitySchemes/security; POST tasks/get without credentials returned a JSON-RPC -32001 (not a 401/403); agent/getAuthenticatedExtendedCard returns -32603 \"Authenticated card not supported\"\n- surface: MCP servers (four onrender.com endpoints)\n  auth: none\n  evidence: 'READMEs: \"API 키 불필요\" (news); data servers read DATA_GO_KR_API_KEY / ECOS_API_KEY from the server environment (render.yaml envVars sync false) and expose no credential to the client; endpoints were suspended (503) so no live challenge could be observed'\n- surface: self-hosted MCP (local stdio)\n  auth: operator-supplied upstream keys\n  evidence: '.env.example lists DATA_GO_KR_API_KEY and ECOS_API_KEY (free keys from data.go.kr and ecos.bok.or.kr); these authenticate the server to the Korean government upstreams, not\
  \ the client to the server'\nupstream_credentials:\n- {name: DATA_GO_KR_API_KEY, issuer: https://www.data.go.kr, used_by: [korean-public-data-mcp, korean-stock-mcp, korean-agriculture-mcp], note: free; instant approval per README}\n- {name: ECOS_API_KEY, issuer: https://ecos.bok.or.kr/api, used_by: [korean-public-data-mcp], note: free}\nprobes:\n- {url: https://publicdata-agent.songt50.us/, method: POST tasks/get (no credentials), status: 200, response: '{\"error\":{\"code\":-32001,\"message\":\"Task not found\"}}'}\n- {url: https://news-agent.songt50.us/, method: POST tasks/get (no credentials), status: 200, response: '{\"error\":{\"code\":-32001,\"message\":\"Task not found\"}}'}\n- {url: https://publicdata-agent.songt50.us/.well-known/oauth-protected-resource, status: 404}\n- {url: https://publicdata-agent.songt50.us/.well-known/oauth-authorization-server, status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/songt50-us/refs/heads/main/authentication/songt50-us-authentication.yml
summary_line: 0 schemes
tags:
- Agents
- A2A
- MCP
- Open Data
- Government Data
- News
- Weather
- Air Quality
- Real Estate
- Economic Statistics
- Stock Market
- Agriculture
- South Korea
- Agent-Native
---
