---
anonymous_access: false
api_key_in:
- header
- query
auth_types:
- oauth2
- openIdConnect
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 12
method: searched
name: Cequence Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- tokenExchange
overview: Cequence Security secures its APIs with oauth2, openIdConnect, apiKey, and http across 12 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and tokenExchange flow(s).
provider_name: Cequence Security
provider_slug: cequence
scheme_count: 12
schemes:
- authorization_url: https://mcp.aigateway.cequence.ai/authorize
  bearer_methods_supported:
  - header
  dynamic_client_registration: true
  flow: authorizationCode
  issuer: https://mcp.aigateway.cequence.ai
  name: MCP OAuth 2.1 (first-party endpoint)
  pkce: S256
  plane: inbound
  registration_url: https://mcp.aigateway.cequence.ai/register
  resource: https://mcp.aigateway.cequence.ai/mcp
  revocation_url: https://mcp.aigateway.cequence.ai/revoke
  scopes:
  - openid
  - profile
  - email
  - descope.claims
  - descope.custom_claims
  sources:
  - well-known/cequence-oauth-authorization-server.json
  - well-known/cequence-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - none
  token_url: https://mcp.aigateway.cequence.ai/token
  type: oauth2
- description: Browser-based single sign-on for a human-driven agent session. Supported identity providers documented as Microsoft Entra ID (including an Entra proxy mode), Google Workspace, Okta and GitLab. SSO groups map to AI Gateway Teams, which gate access to MCP servers and Agent Personas.
  name: Interactive SSO
  plane: inbound
  sources:
  - https://docs.aigateway.cequence.ai/docs/sso-mcp
  type: openIdConnect
- description: A non-interactive credential issued per agent, used where a CI/CD pipeline, an SDK client or a headless runtime cannot complete a browser OAuth flow. Enforced per LLM Registry entry and per Agent Persona.
  in: header
  name: Agent Access Key
  plane: inbound
  sources:
  - https://docs.aigateway.cequence.ai/docs/llm-registry/
  type: apiKey
- bearer_format: JWT
  configuration_inputs:
  - jwks_url
  - issuer
  - audience
  description: The gateway validates a caller-supplied JWT against a configured JWKS URL, expected issuer and expected audience, then passes the caller identity through so the upstream call runs under the real user.
  name: JWT validation (passthrough)
  plane: inbound
  scheme: bearer
  type: http
- description: A tenant-scoped bearer token for the Cequence control-plane REST API. Documented by the first-party CLI, which posts a spec bundle to POST /api/v2/mcp-specs using --api-url, --tenant and --api-token (env fallbacks CEQUENCE_API_URL, CEQUENCE_TENANT_ID, CEQUENCE_API_TOKEN). The control-plane base URL is per-deployment; Cequence publishes no OpenAPI for it.
  name: Control-plane bearer token
  plane: inbound
  scheme: bearer
  sources:
  - https://www.npmjs.com/package/@cequenceai/mcp-cli
  type: http
- callback: https://auth.aigateway.cequence.ai/v1/outbound/oauth/callback
  description: Per-user upstream authorization — each person connects an app (GitHub, Slack, Jira, Salesforce, Google Workspace) once and the gateway stores and refreshes that user's token, so upstream audit trails show the real user rather than a shared bot account.
  flow: authorizationCode
  name: OAuth 2.1 Authorization (upstream)
  plane: outbound
  type: oauth2
- configuration_inputs:
  - token_url
  - client_id
  - client_secret
  - scopes
  flow: clientCredentials
  name: OAuth 2.1 Client Credentials (upstream)
  plane: outbound
  type: oauth2
- configuration_inputs:
  - exchange_endpoint
  - client_id
  - client_secret
  - audience
  flow: tokenExchange
  name: Token exchange (on behalf of caller)
  plane: outbound
  type: oauth2
- configuration_inputs:
  - key_name
  - key_value
  - location
  in:
  - header
  - query
  name: API key (upstream)
  plane: outbound
  type: apiKey
- name: Bearer token (upstream)
  plane: outbound
  scheme: bearer
  type: http
- name: Basic authentication (upstream)
  plane: outbound
  scheme: basic
  type: http
- description: The caller's own credential is forwarded unchanged to the upstream application.
  name: Passthrough
  plane: outbound
  type: http
slug: cequence-authentication
source_filename: cequence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.aigateway.cequence.ai/docs/guides/multi-authentication\ndocs: https://docs.aigateway.cequence.ai/docs/guides/multi-authentication\nprobed:\n- url: https://mcp.aigateway.cequence.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-09-05'\n- url: https://mcp.aigateway.cequence.ai/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-09-05'\nnote: >-\n  Cequence publishes no OpenAPI, so this profile is read from the AI Gateway documentation and\n  from the two live OAuth discovery documents served by the first-party MCP endpoint — not\n  derived from securitySchemes. Cequence AI Gateway is unusual in that it has TWO auth planes:\n  INBOUND (how an agent authenticates to the gateway) and OUTBOUND (how the gateway\n  authenticates to the upstream application on the agent's behalf). Both are catalogued below.\nsummary:\n  types: [oauth2, openIdConnect, apiKey, http]\n\
  \  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode, clientCredentials, tokenExchange]\n  planes: [inbound, outbound]\nschemes:\n- name: MCP OAuth 2.1 (first-party endpoint)\n  plane: inbound\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  dynamic_client_registration: true\n  issuer: https://mcp.aigateway.cequence.ai\n  authorization_url: https://mcp.aigateway.cequence.ai/authorize\n  token_url: https://mcp.aigateway.cequence.ai/token\n  registration_url: https://mcp.aigateway.cequence.ai/register\n  revocation_url: https://mcp.aigateway.cequence.ai/revoke\n  token_endpoint_auth_methods_supported: [none]\n  scopes: [openid, profile, email, descope.claims, descope.custom_claims]\n  bearer_methods_supported: [header]\n  resource: https://mcp.aigateway.cequence.ai/mcp\n  sources:\n  - well-known/cequence-oauth-authorization-server.json\n  - well-known/cequence-oauth-protected-resource.json\n- name: Interactive SSO\n  plane: inbound\n  type: openIdConnect\n  description:\
  \ >-\n    Browser-based single sign-on for a human-driven agent session. Supported identity\n    providers documented as Microsoft Entra ID (including an Entra proxy mode), Google\n    Workspace, Okta and GitLab. SSO groups map to AI Gateway Teams, which gate access to MCP\n    servers and Agent Personas.\n  sources: [https://docs.aigateway.cequence.ai/docs/sso-mcp]\n- name: Agent Access Key\n  plane: inbound\n  type: apiKey\n  in: header\n  description: >-\n    A non-interactive credential issued per agent, used where a CI/CD pipeline, an SDK client\n    or a headless runtime cannot complete a browser OAuth flow. Enforced per LLM Registry\n    entry and per Agent Persona.\n  sources: [https://docs.aigateway.cequence.ai/docs/llm-registry/]\n- name: JWT validation (passthrough)\n  plane: inbound\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    The gateway validates a caller-supplied JWT against a configured JWKS URL, expected issuer\n    and expected audience,\
  \ then passes the caller identity through so the upstream call runs\n    under the real user.\n  configuration_inputs: [jwks_url, issuer, audience]\n- name: Control-plane bearer token\n  plane: inbound\n  type: http\n  scheme: bearer\n  description: >-\n    A tenant-scoped bearer token for the Cequence control-plane REST API. Documented by the\n    first-party CLI, which posts a spec bundle to POST /api/v2/mcp-specs using --api-url,\n    --tenant and --api-token (env fallbacks CEQUENCE_API_URL, CEQUENCE_TENANT_ID,\n    CEQUENCE_API_TOKEN). The control-plane base URL is per-deployment; Cequence publishes no\n    OpenAPI for it.\n  sources: [https://www.npmjs.com/package/@cequenceai/mcp-cli]\n- name: OAuth 2.1 Authorization (upstream)\n  plane: outbound\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    Per-user upstream authorization — each person connects an app (GitHub, Slack, Jira,\n    Salesforce, Google Workspace) once and the gateway stores and refreshes that user's\
  \ token,\n    so upstream audit trails show the real user rather than a shared bot account.\n  callback: https://auth.aigateway.cequence.ai/v1/outbound/oauth/callback\n- name: OAuth 2.1 Client Credentials (upstream)\n  plane: outbound\n  type: oauth2\n  flow: clientCredentials\n  configuration_inputs: [token_url, client_id, client_secret, scopes]\n- name: Token exchange (on behalf of caller)\n  plane: outbound\n  type: oauth2\n  flow: tokenExchange\n  configuration_inputs: [exchange_endpoint, client_id, client_secret, audience]\n- name: API key (upstream)\n  plane: outbound\n  type: apiKey\n  in: [header, query]\n  configuration_inputs: [key_name, key_value, location]\n- name: Bearer token (upstream)\n  plane: outbound\n  type: http\n  scheme: bearer\n- name: Basic authentication (upstream)\n  plane: outbound\n  type: http\n  scheme: basic\n- name: Passthrough\n  plane: outbound\n  type: http\n  description: The caller's own credential is forwarded unchanged to the upstream application.\n\
  credential_storage: >-\n  API keys, tokens and OAuth secrets entered in the portal are encrypted and held in the\n  platform secret manager (provider statement, multi-authentication guide).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cequence/refs/heads/main/authentication/cequence-authentication.yml
summary_line: oauth2/openIdConnect/apiKey/http · 12 schemes
tags:
- AI Protection
- API Discovery
- API Security
- Application Security
- Attack Surface
- Bot Management
- Business Logic Abuse
- CNAPP
- Cybersecurity
- Fraud
- Unified API Protection
---
