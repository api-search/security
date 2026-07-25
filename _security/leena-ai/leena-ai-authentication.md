---
api_key_in: []
api_specs:
- filename: leena-ai-analytics-api-openapi.yml
  format: yaml
  label: Leena AI Analytics API
  slug: leena-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-analytics-api-openapi.yml
- filename: leena-ai-aop-api-openapi.yml
  format: yaml
  label: Leena AI AOP API
  slug: leena-ai-aop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-aop-api-openapi.yml
- filename: leena-ai-audit-logs-api-openapi.yml
  format: yaml
  label: Leena AI Audit Logs API
  slug: leena-ai-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-audit-logs-api-openapi.yml
- filename: leena-ai-authentication-api-openapi.yml
  format: yaml
  label: Leena AI Authentication API
  slug: leena-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-authentication-api-openapi.yml
- filename: leena-ai-knowledge-articles-api-openapi.yml
  format: yaml
  label: Leena AI Knowledge Articles API
  slug: leena-ai-knowledge-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-knowledge-articles-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Leena Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leena AI declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Leena AI
provider_slug: leena-ai
scheme_count: 4
schemes:
- applies_to:
  - openapi/leena-ai-aop-openapi.yml
  - openapi/leena-ai-audit-logs-openapi.yml
  claims:
  - name: botId
    note: The Audit Logs API rejects a token that lacks a `botId` claim with 401 "Token is missing botId".
    required: true
  - name: id
    note: The rate limiter keys its per-client window on the JWT `id` claim.
  client_authentication: client_secret_basic
  description: Resource owner password credentials grant. Client authentication is HTTP Basic with the base64 of `clientId:clientSecret`; the body carries `username`, `password` and `grant_type=password`.
  expires_in: 3600
  flow: password
  header: 'Authorization: Bearer <access_token>'
  id: oauth2_password
  refresh_token: true
  scopes_supported:
  - audit-logs:read
  token_endpoint: https://<region-code>-acl.leena.ai/api/v1.0/oauth/token
  token_endpoint_default_region: https://acl.leena.ai/api/v1.0/oauth/token
  token_type: Bearer
  type: oauth2
- applies_to:
  - mcp/leena-ai-mcp.yml
  description: MCP and A2A both use OAuth 2.0 with the access token sent as a Bearer token in the Authorization header. The client ID and secret are generated from Orchestrator Settings, and an HTTPS redirect URI must be registered.
  id: oauth2_mcp
  redirect_uri_required: true
  redirect_uri_scheme: https
  type: oauth2
- applies_to:
  - openapi/leena-ai-knowledge-management-openapi.yml
  description: The Knowledge Management REST connector obtains a temporary bearer token from `/api/v1.0/oauth/token` using a clientId, clientSecret, username and password supplied by a Leena AI representative.
  guidance: Leena AI recommends implementing token refresh logic within your middleware because of the 30-minute default validity.
  id: km_bearer
  scheme: bearer
  token_validity_minutes: 30
  type: http
- description: Internal Leena AI services and inbound webhook targets can authenticate with the Leena App Secret key, managed within the Leena AI platform. Webhook authentication additionally supports No Auth, Basic Authentication and Bearer Token.
  id: leena_app_secret
  source: https://docs.leena.ai/docs/rest-api
  type: apiKey
slug: leena-ai-authentication
source_filename: leena-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.leena.ai/docs/external-aop-api-authentication-usage-guide
source_yaml: "generated: '2026-07-19'\nmethod: searched\ndocs: https://docs.leena.ai/docs/external-aop-api-authentication-usage-guide\nsources:\n  - https://docs.leena.ai/docs/external-aop-api-authentication-usage-guide\n  - https://docs.leena.ai/docs/audit-logs-external-api-authentication-usage-guide-beta\n  - https://docs.leena.ai/docs/rest\n  - https://docs.leena.ai/docs/leena-ai-mcp-server\nsummary: >-\n  Leena AI's external APIs authenticate with OAuth 2.0 using the resource owner password\n  credentials grant. The client authenticates to the regional ACL token endpoint with HTTP\n  Basic (base64 of clientId:clientSecret) and posts a username, password and\n  grant_type=password. The response carries a Bearer access token, a refresh token, and an\n  expires_in of 3600 seconds. Credentials are issued by a Leena AI representative or, for\n  MCP/A2A, self-generated from Orchestrator Settings. There is no public self-service\n  signup for API credentials.\nschemes:\n  - id: oauth2_password\n\
  \    type: oauth2\n    flow: password\n    description: >-\n      Resource owner password credentials grant. Client authentication is HTTP Basic with\n      the base64 of `clientId:clientSecret`; the body carries `username`, `password` and\n      `grant_type=password`.\n    token_endpoint: 'https://<region-code>-acl.leena.ai/api/v1.0/oauth/token'\n    token_endpoint_default_region: https://acl.leena.ai/api/v1.0/oauth/token\n    client_authentication: client_secret_basic\n    token_type: Bearer\n    header: 'Authorization: Bearer <access_token>'\n    expires_in: 3600\n    refresh_token: true\n    scopes_supported:\n      - audit-logs:read\n    applies_to:\n      - openapi/leena-ai-aop-openapi.yml\n      - openapi/leena-ai-audit-logs-openapi.yml\n    claims:\n      - name: botId\n        required: true\n        note: >-\n          The Audit Logs API rejects a token that lacks a `botId` claim with 401\n          \"Token is missing botId\".\n      - name: id\n        note: The rate limiter\
  \ keys its per-client window on the JWT `id` claim.\n  - id: oauth2_mcp\n    type: oauth2\n    description: >-\n      MCP and A2A both use OAuth 2.0 with the access token sent as a Bearer token in the\n      Authorization header. The client ID and secret are generated from Orchestrator\n      Settings, and an HTTPS redirect URI must be registered.\n    redirect_uri_required: true\n    redirect_uri_scheme: https\n    applies_to:\n      - mcp/leena-ai-mcp.yml\n  - id: km_bearer\n    type: http\n    scheme: bearer\n    description: >-\n      The Knowledge Management REST connector obtains a temporary bearer token from\n      `/api/v1.0/oauth/token` using a clientId, clientSecret, username and password\n      supplied by a Leena AI representative.\n    token_validity_minutes: 30\n    guidance: >-\n      Leena AI recommends implementing token refresh logic within your middleware because\n      of the 30-minute default validity.\n    applies_to:\n      - openapi/leena-ai-knowledge-management-openapi.yml\n\
  \  - id: leena_app_secret\n    type: apiKey\n    description: >-\n      Internal Leena AI services and inbound webhook targets can authenticate with the\n      Leena App Secret key, managed within the Leena AI platform. Webhook authentication\n      additionally supports No Auth, Basic Authentication and Bearer Token.\n    source: https://docs.leena.ai/docs/rest-api\ncredential_issuance:\n  self_service: false\n  process: >-\n    API credentials (clientId, clientSecret, username, password) are provisioned by a Leena\n    AI representative. MCP/A2A OAuth clients are generated by a tenant administrator in\n    Orchestrator Settings.\nsso:\n  supported: true\n  note: >-\n    Leena AI documents enterprise identity integrations including Okta for platform SSO.\n  source: https://docs.leena.ai/docs/okta\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/authentication/leena-ai-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Ai Ml
- Agentic AI
- Artificial Intelligence
- Enterprise Software
- Human Resources
- IT Service Management
- Employee Experience
- Workflow Automation
- Conversational AI
- Model Context Protocol
- Knowledge Management
---
