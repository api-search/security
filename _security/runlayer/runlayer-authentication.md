---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Runlayer Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- tokenExchange
overview: Runlayer secures its APIs with apiKey, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and tokenExchange flow(s).
provider_name: Runlayer
provider_slug: runlayer
scheme_count: 4
schemes:
- in: header
  key_prefix: rl_
  name: RunlayerApiKey
  notes: Personal API keys authenticate as the creating user; Organization API keys authenticate as the workspace and are role-scoped. Send as the x-runlayer-api-key header (NOT a bearer token).
  parameter_name: x-runlayer-api-key
  scopes_by_role:
  - Deploy
  - Shadow AI Scan
  - Security Scan
  type: apiKey
- flow: clientCredentials
  grant: client_credentials
  name: AgentAccountM2M
  notes: Agent Accounts (beta) authenticate with a Client ID + Client Secret to mint a machine-to-machine agent JWT (1h TTL), acting as the agent itself.
  token_url: /api/v1/oauth/token
  type: oauth2
- flow: tokenExchange
  grant: urn:ietf:params:oauth:grant-type:token-exchange
  name: AgentAccountOBO
  notes: 'On-Behalf-Of: exchange the agent JWT (actor_token) for an OBO token bound to a subject user; enforces the intersection of agent + user policies.'
  standard: RFC 8693
  token_url: /api/v1/oauth/token
  type: oauth2
- host: https://oauth.runlayer.com
  name: OAuthBroker
  notes: Centralized OAuth/OIDC broker for upstream vendor connectors (GitHub, Asana, Ramp, Datadog, …). PKCE on the MCP<->Broker hop and Broker<->Vendor hop when supported; Dynamic Client Registration.
  standards:
  - OAuth 2.0
  - OIDC
  - PKCE
  - DCR
  type: openIdConnect
slug: runlayer-authentication
source_filename: runlayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.runlayer.com/platform-api ; https://docs.runlayer.com/platform-agent-accounts ; https://docs.runlayer.com/oauth-broker ; https://docs.runlayer.com/connecting-clients\ndocs: https://docs.runlayer.com/platform-api\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials, tokenExchange]\nschemes:\n- name: RunlayerApiKey\n  type: apiKey\n  in: header\n  parameter_name: x-runlayer-api-key\n  key_prefix: rl_\n  scopes_by_role:\n  - Deploy\n  - Shadow AI Scan\n  - Security Scan\n  notes: >-\n    Personal API keys authenticate as the creating user; Organization API keys\n    authenticate as the workspace and are role-scoped. Send as the\n    x-runlayer-api-key header (NOT a bearer token).\n- name: AgentAccountM2M\n  type: oauth2\n  flow: clientCredentials\n  token_url: /api/v1/oauth/token\n  grant: client_credentials\n  notes: >-\n    Agent Accounts (beta) authenticate\
  \ with a Client ID + Client Secret to mint\n    a machine-to-machine agent JWT (1h TTL), acting as the agent itself.\n- name: AgentAccountOBO\n  type: oauth2\n  flow: tokenExchange\n  token_url: /api/v1/oauth/token\n  grant: urn:ietf:params:oauth:grant-type:token-exchange\n  standard: RFC 8693\n  notes: >-\n    On-Behalf-Of: exchange the agent JWT (actor_token) for an OBO token bound to\n    a subject user; enforces the intersection of agent + user policies.\n- name: OAuthBroker\n  type: openIdConnect\n  host: https://oauth.runlayer.com\n  standards: [OAuth 2.0, OIDC, PKCE, DCR]\n  notes: >-\n    Centralized OAuth/OIDC broker for upstream vendor connectors (GitHub, Asana,\n    Ramp, Datadog, …). PKCE on the MCP<->Broker hop and Broker<->Vendor hop when\n    supported; Dynamic Client Registration.\nerror_semantics:\n  '401': Missing or invalid API key / unauthenticated request.\n  '403': Key role lacks access to the endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runlayer/refs/heads/main/authentication/runlayer-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 4 schemes
tags:
- Company
- AI
- AI Agents
- MCP
- Model Context Protocol
- API Gateway
- Security
- Governance
- Identity
- Observability
- Enterprise
---
