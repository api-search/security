---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Monte Carlo Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monte Carlo declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Monte Carlo
provider_slug: monte-carlo-data
scheme_count: 6
schemes:
- description: Key ID + secret pair. Keys are generated from 42 cryptographically secure random bytes, base64-encoded to a 56-character string. Secret is shown once. Personal and account-level key types; account-level creation is permission-gated (Account Owners by default).
  docs: https://docs.getmontecarlo.com/docs/api-authentication#creating-an-api-key
  id: mcd-api-key
  in: header
  names:
  - x-mcd-id
  - x-mcd-token
  rotation: Maximum expiration capped at one year for personal keys, MCP keys and personal OAuth clients; service credentials remain long-lived.
  surface: GraphQL API (https://api.getmontecarlo.com/graphql)
  type: apiKey
- api_url: https://api.getmontecarlo.com/graphql
  description: 'Machine-to-machine authentication. Two client kinds: personal clients (act as the creating user) and service clients (account-level, scoped by authorization groups). Each client holds up to two secrets for zero-downtime rotation. The instance-routing scope names the deployment (us1, eu1, ...).'
  docs: https://docs.getmontecarlo.com/docs/api-authentication#authenticating-with-oauth-client-credentials
  flow: clientCredentials
  id: oauth2-client-credentials
  scopes:
  - https://api.getmontecarlo.com/access
  - https://instance.getmontecarlo.com/{instance_id}
  surface: GraphQL API, Python SDK, CLI
  token_format: JWT bearer
  token_url: https://api.getmontecarlo.com/oauth2/token
  type: oauth2
- authorization_endpoint: https://auth.getmontecarlo.com/oauth2/authorize
  authorization_server: https://auth.getmontecarlo.com
  description: 'OAuth 2.1 with Dynamic Client Registration for MCP clients. Probed live: the MCP endpoint returns a conformant RFC 9728 challenge pointing at its protected-resource metadata. Requires an Editor role or above.'
  device_authorization_endpoint: https://auth.getmontecarlo.com/oauth2/device_authorization
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  id: oauth2.1-mcp
  introspection_endpoint: https://auth.getmontecarlo.com/oauth2/introspection
  issuer: https://auth.getmontecarlo.com
  jwks_uri: https://auth.getmontecarlo.com/oauth2/jwks
  method: probed
  pkce: S256
  registration_endpoint: https://auth.getmontecarlo.com/oauth2/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  surface: MCP server (https://mcp.getmontecarlo.com/mcp)
  token_endpoint: https://auth.getmontecarlo.com/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://auth.getmontecarlo.com/oauth2/userinfo
- description: Scoped credentials that work ONLY with the MCP server. Standard API keys are rejected. Created via UI, `montecarlo mcp create-key`, or the createMcpIntegrationKey GraphQL mutation (CLI v0.141.4+).
  docs: https://docs.getmontecarlo.com/docs/mcp-server
  format: 'Authorization: Bearer <KEY_ID>:<KEY_SECRET>'
  id: mcp-server-key
  in: header
  names:
  - Authorization
  - x-mcd-id
  - x-mcd-token
  surface: MCP server
  type: apiKey
- description: A dedicated integration key with scope `Ingestion`, optionally bound to specific warehouseIds. A standard Monte Carlo API key will not work. Created with the createIntegrationKey GraphQL mutation or `montecarlo integrations create-key --scope Ingestion`.
  docs: https://docs.getmontecarlo.com/docs/push-ingest-api#prerequisites
  id: ingestion-key
  in: header
  names:
  - x-mcd-id
  - x-mcd-token
  scope_value: Ingestion
  surface: Push Ingest API (https://integrations.getmontecarlo.com)
  type: apiKey
- algorithm: HMAC-SHA-512
  description: Outbound webhook calls from Monte Carlo are optionally signed with a customer-supplied shared secret so the receiver can verify authenticity.
  direction: inbound-to-customer
  docs: https://docs.getmontecarlo.com/docs/webhooks
  header: x-mcd-signature
  id: webhook-hmac
  type: signature
slug: monte-carlo-data-authentication
source_filename: monte-carlo-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://docs.getmontecarlo.com/docs/api-authentication,\n  https://docs.getmontecarlo.com/docs/push-ingest-api,\n  https://docs.getmontecarlo.com/docs/mcp-server,\n  plus live reads of https://auth.getmontecarlo.com/.well-known/oauth-authorization-server\n  and https://mcp.getmontecarlo.com/.well-known/oauth-protected-resource/mcp\ndocs: https://docs.getmontecarlo.com/docs/api-authentication\nprovider: Monte Carlo\nproviderId: monte-carlo-data\nnote: >-\n  Monte Carlo publishes no OpenAPI, so this profile is derived from the auth\n  documentation and from live OAuth metadata rather than from securitySchemes.\n  Four distinct credential families exist and they are NOT interchangeable —\n  the docs are explicit that a standard API key will not work against the MCP\n  server or the Push Ingest API.\nschemes:\n  - id: mcd-api-key\n    type: apiKey\n    in: header\n    names:\n      - x-mcd-id\n      - x-mcd-token\n    surface:\
  \ GraphQL API (https://api.getmontecarlo.com/graphql)\n    description: >-\n      Key ID + secret pair. Keys are generated from 42 cryptographically secure\n      random bytes, base64-encoded to a 56-character string. Secret is shown\n      once. Personal and account-level key types; account-level creation is\n      permission-gated (Account Owners by default).\n    rotation: >-\n      Maximum expiration capped at one year for personal keys, MCP keys and\n      personal OAuth clients; service credentials remain long-lived.\n    docs: https://docs.getmontecarlo.com/docs/api-authentication#creating-an-api-key\n  - id: oauth2-client-credentials\n    type: oauth2\n    flow: clientCredentials\n    surface: GraphQL API, Python SDK, CLI\n    token_url: https://api.getmontecarlo.com/oauth2/token\n    api_url: https://api.getmontecarlo.com/graphql\n    token_format: JWT bearer\n    scopes:\n      - https://api.getmontecarlo.com/access\n      - https://instance.getmontecarlo.com/{instance_id}\n\
  \    description: >-\n      Machine-to-machine authentication. Two client kinds: personal clients\n      (act as the creating user) and service clients (account-level, scoped by\n      authorization groups). Each client holds up to two secrets for\n      zero-downtime rotation. The instance-routing scope names the deployment\n      (us1, eu1, ...).\n    docs: https://docs.getmontecarlo.com/docs/api-authentication#authenticating-with-oauth-client-credentials\n  - id: oauth2.1-mcp\n    type: oauth2\n    flow: authorizationCode\n    pkce: S256\n    dynamic_client_registration: true\n    surface: MCP server (https://mcp.getmontecarlo.com/mcp)\n    authorization_server: https://auth.getmontecarlo.com\n    issuer: https://auth.getmontecarlo.com\n    authorization_endpoint: https://auth.getmontecarlo.com/oauth2/authorize\n    token_endpoint: https://auth.getmontecarlo.com/oauth2/token\n    registration_endpoint: https://auth.getmontecarlo.com/oauth2/register\n    introspection_endpoint: https://auth.getmontecarlo.com/oauth2/introspection\n\
  \    device_authorization_endpoint: https://auth.getmontecarlo.com/oauth2/device_authorization\n    jwks_uri: https://auth.getmontecarlo.com/oauth2/jwks\n    userinfo_endpoint: https://auth.getmontecarlo.com/oauth2/userinfo\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:device_code\n    scopes:\n      - openid\n      - profile\n      - email\n      - offline_access\n    token_endpoint_auth_methods:\n      - none\n      - client_secret_basic\n      - client_secret_post\n    description: >-\n      OAuth 2.1 with Dynamic Client Registration for MCP clients. Probed live:\n      the MCP endpoint returns a conformant RFC 9728 challenge pointing at its\n      protected-resource metadata. Requires an Editor role or above.\n    method: probed\n  - id: mcp-server-key\n    type: apiKey\n    in: header\n    names:\n      - Authorization\n      - x-mcd-id\n      - x-mcd-token\n    format: 'Authorization: Bearer\
  \ <KEY_ID>:<KEY_SECRET>'\n    surface: MCP server\n    description: >-\n      Scoped credentials that work ONLY with the MCP server. Standard API keys\n      are rejected. Created via UI, `montecarlo mcp create-key`, or the\n      createMcpIntegrationKey GraphQL mutation (CLI v0.141.4+).\n    docs: https://docs.getmontecarlo.com/docs/mcp-server\n  - id: ingestion-key\n    type: apiKey\n    in: header\n    names:\n      - x-mcd-id\n      - x-mcd-token\n    surface: Push Ingest API (https://integrations.getmontecarlo.com)\n    scope_value: Ingestion\n    description: >-\n      A dedicated integration key with scope `Ingestion`, optionally bound to\n      specific warehouseIds. A standard Monte Carlo API key will not work.\n      Created with the createIntegrationKey GraphQL mutation or\n      `montecarlo integrations create-key --scope Ingestion`.\n    docs: https://docs.getmontecarlo.com/docs/push-ingest-api#prerequisites\n  - id: webhook-hmac\n    type: signature\n    direction: inbound-to-customer\n\
  \    algorithm: HMAC-SHA-512\n    header: x-mcd-signature\n    description: >-\n      Outbound webhook calls from Monte Carlo are optionally signed with a\n      customer-supplied shared secret so the receiver can verify authenticity.\n    docs: https://docs.getmontecarlo.com/docs/webhooks\nsso:\n  supported: true\n  note: >-\n    SSO with enforced password-login disablement, single-use recovery codes,\n    and a per-account IP allowlist on the redeem endpoint.\n  docs: https://docs.getmontecarlo.com/docs/sso-recovery-codes\nnetwork_access_control:\n  supported: true\n  scopes:\n    - MCP\n    - API\n    - Ingestion\n    - UI\n    - Agent\n    - OpenTelemetry\n  docs: https://docs.getmontecarlo.com/docs/network-access-control\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monte-carlo-data/refs/heads/main/authentication/monte-carlo-data-authentication.yml
summary_line: 6 schemes
tags:
- AIOps
- Data Observability
- Data Quality
- Data Lineage
- Agent Observability
- Monitoring
- GraphQL
- MCP
- OpenTelemetry
- Data Engineering
---
