---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cloutjam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CloutJam secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CloutJam
provider_slug: cloutjam
scheme_count: 2
schemes:
- audience: power users, scripted/CLI workflows
  bearer_prefix: cd_pat_
  name: personalAccessToken
  scheme: bearer
  sources:
  - https://www.cloutdesk.com/agent-platform
  type: http
- audience: organization-wide installs
  flow: authorizationCode
  name: oauth2
  scopes_documented:
  - campaigns
  - collaborations
  - agreements:write
  sources:
  - https://www.cloutdesk.com/agent-platform
  type: oauth2
slug: cloutjam-authentication
source_filename: cloutjam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.cloutdesk.com/agent-platform\nstatus: beta\nnotes: >-\n  CloutDesk's Agent Platform page documents two auth mechanisms for its\n  announced (Beta) REST API and MCP server. No OpenAPI securitySchemes were\n  available to derive from (no spec published); this profile is searched from\n  the vendor page.\nsummary:\n  types: [http, oauth2]\n  http_bearer: true\n  oauth2_flows: [authorizationCode]\n  scope_gated: true\nschemes:\n  - name: personalAccessToken\n    type: http\n    scheme: bearer\n    bearer_prefix: 'cd_pat_'\n    audience: power users, scripted/CLI workflows\n    sources: [https://www.cloutdesk.com/agent-platform]\n  - name: oauth2\n    type: oauth2\n    flow: authorizationCode\n    audience: organization-wide installs\n    scopes_documented: [campaigns, collaborations, 'agreements:write']\n    sources: [https://www.cloutdesk.com/agent-platform]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloutjam/refs/heads/main/authentication/cloutjam-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Influencer Marketing
- Creator Management
- Creator Economy
- Marketing
- Agentic AI
- Agents
---
