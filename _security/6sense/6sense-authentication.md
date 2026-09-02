---
api_key_in:
- header
- query
- body
api_specs:
- filename: 6sense-company-api-openapi.yml
  format: yaml
  label: 6sense Company API
  slug: 6sense-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-api-openapi.yml
- filename: 6sense-enrichment-api-openapi.yml
  format: yaml
  label: 6sense Enrichment API
  slug: 6sense-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-enrichment-api-openapi.yml
- filename: 6sense-people-api-openapi.yml
  format: yaml
  label: 6sense People API
  slug: 6sense-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-api-openapi.yml
- filename: 6sense-scoring-api-openapi.yml
  format: yaml
  label: 6sense Scoring API
  slug: 6sense-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-scoring-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: 6Sense Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: 6sense secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: 6sense
provider_slug: 6sense
scheme_count: 4
schemes:
- description: 'Org-level 6sense API token, a randomly generated 40-character alphanumeric key. Tokens are scoped to an API GROUP rather than to endpoints or data: a Company Identification token only works on the Company Identification API, a 6sense Credits token only on the Enrichment APIs, and so on.'
  format: Token <api_token>
  in: header
  management:
    console: 6sense platform Settings > API Token management
    limit: No published cap on the number of tokens per org.
    revocation: Tokens can be deleted from the console; usage history is retained for 12 months.
    roles_none:
    - Insights
    - Sales
    roles_read:
    - Marketing
    - View only
    roles_write:
    - Primary Admin
    - Admin
    - Operations
    rotation_guidance: 6sense recommends rotating API tokens every 90 days.
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/6sense-scribe-openapi.json
  - openapi/6sense-company-api-openapi.yml
  - openapi/6sense-enrichment-api-openapi.yml
  - openapi/6sense-people-api-openapi.yml
  token_groups:
  - credit_model: API Credits
    extras: Allowed-domains allowlist can be attached to restrict where the token may be used.
    group: Company Identification API
    self_service: true
  - applies_to:
    - People Enrichment API
    - Company Firmographics API
    - Lead Scoring and Firmographics API
    credit_model: 6sense Credits
    group: 6sense Credits (Enrichment)
    self_service: true
  - credit_model: none
    group: Lead Scoring API
    requires: Predictive or Advanced package
    self_service: true
  - credit_model: none
    group: Segments API
    note: Issued only to approved partners over email or a support ticket; never visible in the platform UI.
    self_service: false
  - credit_model: none
    group: Sales Intelligence App
    note: Revenue AI for Sales customers only; obtained through support.
    self_service: false
  type: apiKey
- description: The securityScheme name used in the provider-published Scribe OpenAPI at https://scribe.6sense.com/openapi.json. Same credential and same header as TokenAuth above; only the scheme name differs between the published spec and the API Portal documentation.
  in: header
  name: API_KEY
  parameter: Authorization
  sources:
  - openapi/6sense-scribe-openapi.json
  type: apiKey
- description: Per-user OAuth for the remote MCP server at https://api.6sense.com/mcp. Discovered anonymously via RFC 9728 protected-resource metadata advertised in the WWW-Authenticate header of an unauthenticated MCP request. Supports dynamic client registration, PKCE (S256) and DPoP.
  detail: scopes/6sense-scopes.yml
  flows:
  - authorizationUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/authorize
    flow: authorizationCode
    scopes:
      mcp:use: Call the 6sense MCP server on behalf of the consenting user.
    tokenUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token
  - flow: clientCredentials
    tokenUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token
  name: 6sense Agentic OAuth (MCP)
  sources:
  - well-known/6sense-oauth-authorization-server.json
  - well-known/6sense-oauth-protected-resource-mcp.json
  type: oauth2
- alternate_in: body
  alternate_parameter: token
  description: The AI Email (formerly Conversational Email, formerly Saleswhale) API at https://engage-api.saleswhale.com/api/{version}/ authenticates with a token passed either as a ?token= query parameter or as a top-level "token" property in the JSON request body. There is no header-based option documented. A query parameter credential is logged by intermediaries and proxies by default, so this is materially weaker than the header token used by the core data APIs.
  docs: https://docs.saleswhale.com/
  in: query
  name: Saleswhale token (AI Email)
  parameter: token
  sources:
  - https://docs.saleswhale.com/
  type: apiKey
slug: 6sense-authentication
source_filename: 6sense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/6sense-scribe-openapi.json, openapi/6sense-company-api-openapi.yml,\n  openapi/6sense-enrichment-api-openapi.yml, openapi/6sense-people-api-openapi.yml,\n  well-known/6sense-oauth-authorization-server.json\ndocs:\n- https://api.6sense.com/docs/\n- https://support.6sense.com/docs/api-credits-api-tokens\n- https://support.6sense.com/docs/set-up-the-6sense-mcp-in-claude\nnote: >-\n  6sense runs three separate authentication regimes, and which one applies is\n  decided by which product you are calling — not by which endpoint. The public\n  data APIs use a 40-character org-level API token in the Authorization header;\n  the remote MCP server uses per-user OAuth 2.1 with dynamic client registration;\n  and the acquired AI Email (Saleswhale) API uses a token passed as a query\n  parameter or JSON body property, which is the weakest of the three.\n\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  -\
  \ query\n  - body\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <api_token>'\n  description: >-\n    Org-level 6sense API token, a randomly generated 40-character alphanumeric\n    key. Tokens are scoped to an API GROUP rather than to endpoints or data:\n    a Company Identification token only works on the Company Identification API,\n    a 6sense Credits token only on the Enrichment APIs, and so on.\n  token_groups:\n  - group: Company Identification API\n    self_service: true\n    credit_model: API Credits\n    extras: Allowed-domains allowlist can be attached to restrict where the token may be used.\n  - group: 6sense Credits (Enrichment)\n    self_service: true\n    credit_model: 6sense Credits\n    applies_to:\n    - People Enrichment API\n    - Company Firmographics API\n    - Lead Scoring and Firmographics API\n  - group: Lead Scoring API\n    self_service:\
  \ true\n    credit_model: none\n    requires: Predictive or Advanced package\n  - group: Segments API\n    self_service: false\n    credit_model: none\n    note: Issued only to approved partners over email or a support ticket; never visible in the platform UI.\n  - group: Sales Intelligence App\n    self_service: false\n    credit_model: none\n    note: Revenue AI for Sales customers only; obtained through support.\n  management:\n    console: 6sense platform Settings > API Token management\n    roles_write:\n    - Primary Admin\n    - Admin\n    - Operations\n    roles_read:\n    - Marketing\n    - View only\n    roles_none:\n    - Insights\n    - Sales\n    rotation_guidance: 6sense recommends rotating API tokens every 90 days.\n    revocation: Tokens can be deleted from the console; usage history is retained for 12 months.\n    limit: No published cap on the number of tokens per org.\n  sources:\n  - openapi/6sense-scribe-openapi.json\n  - openapi/6sense-company-api-openapi.yml\n  -\
  \ openapi/6sense-enrichment-api-openapi.yml\n  - openapi/6sense-people-api-openapi.yml\n\n- name: API_KEY\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    The securityScheme name used in the provider-published Scribe OpenAPI at\n    https://scribe.6sense.com/openapi.json. Same credential and same header as\n    TokenAuth above; only the scheme name differs between the published spec and\n    the API Portal documentation.\n  sources:\n  - openapi/6sense-scribe-openapi.json\n\n- name: 6sense Agentic OAuth (MCP)\n  type: oauth2\n  description: >-\n    Per-user OAuth for the remote MCP server at https://api.6sense.com/mcp.\n    Discovered anonymously via RFC 9728 protected-resource metadata advertised in\n    the WWW-Authenticate header of an unauthenticated MCP request. Supports\n    dynamic client registration, PKCE (S256) and DPoP.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/authorize\n\
  \    tokenUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token\n    scopes:\n      mcp:use: Call the 6sense MCP server on behalf of the consenting user.\n  - flow: clientCredentials\n    tokenUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token\n  detail: scopes/6sense-scopes.yml\n  sources:\n  - well-known/6sense-oauth-authorization-server.json\n  - well-known/6sense-oauth-protected-resource-mcp.json\n\n- name: Saleswhale token (AI Email)\n  type: apiKey\n  in: query\n  parameter: token\n  alternate_in: body\n  alternate_parameter: token\n  description: >-\n    The AI Email (formerly Conversational Email, formerly Saleswhale) API at\n    https://engage-api.saleswhale.com/api/{version}/ authenticates with a token\n    passed either as a ?token= query parameter or as a top-level \"token\" property\n    in the JSON request body. There is no header-based option documented.\
  \ A query\n    parameter credential is logged by intermediaries and proxies by default, so\n    this is materially weaker than the header token used by the core data APIs.\n  docs: https://docs.saleswhale.com/\n  sources:\n  - https://docs.saleswhale.com/\n\nsecurity_posture:\n  transport: HTTPS only on all hosts probed (TLS 1.3).\n  server_side_only: >-\n    6sense explicitly requires the Enrichment APIs to be server-to-server and\n    warns the token must never be exposed on a public domain. The Company\n    Identification API is the deliberate exception — it is designed for\n    client-side use inside the WebTag, which is why it is the only token group\n    that can be pinned to an allowed-domain list.\n  default_deny_on_settings: >-\n    Score and Segment detail are withheld by default on API token settings and\n    must be explicitly enabled per token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/authentication/6sense-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Account Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- Artificial Intelligence
- Marketing Technology
---
