---
api_key_in: []
api_specs:
- filename: natural-ai-agent-keys-api-openapi.yml
  format: yaml
  label: Natural AI Agent Keys API
  slug: natural-ai-agent-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-agent-keys-api-openapi.yml
- filename: natural-ai-agents-api-openapi.yml
  format: yaml
  label: Natural AI Agents API
  slug: natural-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-agents-api-openapi.yml
- filename: natural-ai-api-keys-api-openapi.yml
  format: yaml
  label: Natural AI API Keys API
  slug: natural-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-api-keys-api-openapi.yml
- filename: natural-ai-approvals-api-openapi.yml
  format: yaml
  label: Natural AI Approvals API
  slug: natural-ai-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-approvals-api-openapi.yml
- filename: natural-ai-customers-api-openapi.yml
  format: yaml
  label: Natural AI Customers API
  slug: natural-ai-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-customers-api-openapi.yml
- filename: natural-ai-events-api-openapi.yml
  format: yaml
  label: Natural AI Events API
  slug: natural-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-events-api-openapi.yml
- filename: natural-ai-external-accounts-api-openapi.yml
  format: yaml
  label: Natural AI External Accounts API
  slug: natural-ai-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-external-accounts-api-openapi.yml
- filename: natural-ai-invitations-api-openapi.yml
  format: yaml
  label: Natural AI Invitations API
  slug: natural-ai-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-invitations-api-openapi.yml
- filename: natural-ai-parties-api-openapi.yml
  format: yaml
  label: Natural AI Parties API
  slug: natural-ai-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-parties-api-openapi.yml
- filename: natural-ai-paymentrequests-api-openapi.yml
  format: yaml
  label: Natural AI PaymentRequests API
  slug: natural-ai-paymentrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-paymentrequests-api-openapi.yml
- filename: natural-ai-payments-api-openapi.yml
  format: yaml
  label: Natural AI Payments API
  slug: natural-ai-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-payments-api-openapi.yml
- filename: natural-ai-transactions-api-openapi.yml
  format: yaml
  label: Natural AI Transactions API
  slug: natural-ai-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-transactions-api-openapi.yml
- filename: natural-ai-transfers-api-openapi.yml
  format: yaml
  label: Natural AI Transfers API
  slug: natural-ai-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-transfers-api-openapi.yml
- filename: natural-ai-wallets-api-openapi.yml
  format: yaml
  label: Natural AI Wallets API
  slug: natural-ai-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-wallets-api-openapi.yml
- filename: natural-ai-webhooks-api-openapi.yml
  format: yaml
  label: Natural AI Webhooks API
  slug: natural-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Natural Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Natural AI secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Natural AI
provider_slug: natural-ai
scheme_count: 2
schemes:
- description: 'Bearer authentication. Send an API key, agent key, or OAuth access token as Authorization: Bearer <credential>.'
  name: HTTPBearer
  scheme: bearer
  source: openapi/natural-ai-openapi-original.json
  type: http
- flows:
  - authorizationUrl: https://api.natural.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.natural.com/oauth/register
    revocationUrl: https://api.natural.com/oauth/revoke
    tokenUrl: https://api.natural.com/oauth/token
    token_endpoint_auth: none
  name: OAuth2
  source: https://api.natural.com/.well-known/oauth-authorization-server
  type: oauth2
slug: natural-ai-authentication
source_filename: natural-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.natural.com/api-reference/authentication\ndocs: https://docs.natural.com/api-reference/authentication\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  credential_modes: [api-key, agent-key, user-scoped-oauth, agent-scoped-oauth]\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  source: openapi/natural-ai-openapi-original.json\n  description: >-\n    Bearer authentication. Send an API key, agent key, or OAuth access token as\n    Authorization: Bearer <credential>.\n- name: OAuth2\n  type: oauth2\n  source: https://api.natural.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.natural.com/oauth/authorize\n    tokenUrl: https://api.natural.com/oauth/token\n    registrationUrl: https://api.natural.com/oauth/register\n    revocationUrl: https://api.natural.com/oauth/revoke\n    pkce:\
  \ S256\n    token_endpoint_auth: none\ncredential_modes:\n- mode: api-key\n  prefix: sk_ntl_\n  format: sk_ntl_{environment}_{secret}\n  environments: [prod]\n  acts_as: your party\n  scopable: true\n- mode: agent-key\n  prefix: ak_ntl_\n  format: ak_ntl_{environment}_{secret}\n  acts_as: one specific bound agent, verified by the credential\n- mode: user-scoped-oauth\n  flow: browser OAuth consent\n  acts_as: the authorizing user/party\n- mode: agent-scoped-oauth\n  flow: browser OAuth consent\n  acts_as: a selected or new agent, verified\nnotes:\n- Credentials are scoped and can never exceed the issuing party's permissions.\n- Keys are high-entropy, shown once, stored only as one-way hashes.\n- OAuth uses 2.1 with PKCE and short-lived access tokens; access tokens signed by AWS KMS.\n- Agent-attributed money movement requires an X-Instance-ID header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/authentication/natural-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Payments
- Agents
- Fintech
- Money Movement
- Wallets
- Agentic Payments
- MCP
---
