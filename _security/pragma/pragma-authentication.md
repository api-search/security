---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pragma Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Pragma secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Pragma
provider_slug: pragma
scheme_count: 3
schemes:
- api: FirstLook External API
  description: Scoped API token created under Settings -> Developer in the FirstLook dashboard. Shown once at creation and cannot be viewed again. Only organization Owners and Developers can manage tokens. Each token carries a note and one or more scopes (see scopes/pragma-scopes.yml). Used to authenticate calls to the FirstLook External API (https://api.firstlook.gg/external).
  in: header
  name: FirstLookApiToken
  type: apiKey
- api: FirstLook External API
  description: OAuth-based login used by the hosted FirstLook MCP server (https://mcp.firstlook.gg/mcp). Users authenticate with their FirstLook account when connecting an AI assistant (Claude, ChatGPT) as a connector.
  flows:
  - authorizationCode
  name: FirstLookMcpOAuth
  scheme: oauth2
  type: oauth2
- api: Pragma Connect
  description: Pragma Connect provides cross-platform player authentication (Steam, Discord, Twitch, PlayStation, Xbox and more) for game clients built on the Pragma Platform. Documented at https://cloud-docs.pragma.gg/ under Features -> Accounts.
  name: PragmaConnectAuth
  type: oauth2
slug: pragma-authentication
source_filename: pragma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.firstlook.gg/developers/api/\ndocs: https://docs.firstlook.gg/developers/api/\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: FirstLookApiToken\n    type: apiKey\n    in: header\n    description: >-\n      Scoped API token created under Settings -> Developer in the FirstLook\n      dashboard. Shown once at creation and cannot be viewed again. Only\n      organization Owners and Developers can manage tokens. Each token carries a\n      note and one or more scopes (see scopes/pragma-scopes.yml). Used to\n      authenticate calls to the FirstLook External API (https://api.firstlook.gg/external).\n    api: FirstLook External API\n  - name: FirstLookMcpOAuth\n    type: oauth2\n    scheme: oauth2\n    flows: [authorizationCode]\n    description: >-\n      OAuth-based login used by the hosted FirstLook MCP server\n      (https://mcp.firstlook.gg/mcp).\
  \ Users authenticate with their FirstLook\n      account when connecting an AI assistant (Claude, ChatGPT) as a connector.\n    api: FirstLook External API\n  - name: PragmaConnectAuth\n    type: oauth2\n    description: >-\n      Pragma Connect provides cross-platform player authentication (Steam,\n      Discord, Twitch, PlayStation, Xbox and more) for game clients built on the\n      Pragma Platform. Documented at https://cloud-docs.pragma.gg/ under Features -> Accounts.\n    api: Pragma Connect\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pragma/refs/heads/main/authentication/pragma-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Infrastructure
- Gaming
- Game Backend
- Live Operations
- Player Accounts
- Authentication
- Commerce
- Playtesting
- Community
- Analytics
- Developer Tools
---
