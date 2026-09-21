---
anonymous_access: false
api_key_in:
- header
- query (deprecated for MCP URLs)
api_specs:
- filename: fodda-ai-openapi.yml
  format: yaml
  label: Fodda Context & Research API
  slug: fodda-context-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fodda-ai/refs/heads/main/openapi/fodda-ai-openapi.yml
auth_types:
- apiKey
- http
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Fodda Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode (PKCE S256)
- deviceCode
- refresh_token
overview: Fodda (PSFK) secures its APIs with apiKey, http, openIdConnect, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode (PKCE S256), deviceCode, and refresh_token flow(s).
provider_name: Fodda (PSFK)
provider_slug: fodda-ai
scheme_count: 5
schemes:
- description: 'Required for all endpoints unless marked public. Issued at app.fodda.ai (Account); free tier $50 of API calls / 100 calls per month with a card on file, then $0.50 per call. Self-serve key rotation at app.fodda.ai (compliance dossier). Copilot Studio guide also accepts Authorization: Bearer <api key>. Autonomous provisioning: POST /api/account/b2b-provision (named on /agents; not in the OpenAPI).'
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/fodda-ai-openapi.yml
  - openapi/fodda-ai-context-delivery-openapi.yml
  - https://www.fodda.ai/llms.txt
  - https://www.fodda.ai/agents
  surfaces:
  - REST
  - MCP (header or personal URL)
  type: apiKey
- bearer_format: spt_... (Stripe Shared Payment Token)
  description: 'Machine Payments Protocol: call any endpoint with no credentials, receive HTTP 402 with the exact price (WWW-Authenticate: stripe-spt amount=<cents> currency=usd), obtain an SPT from Stripe Link, retry with Authorization: Bearer spt_xxx or X-Stripe-SPT: spt_xxx. Price = API-call count × $0.50. Direct REST API only (not MCP). Validate with GET /v1/spt/validate.'
  name: stripeSPT
  scheme: bearer
  sources:
  - openapi/fodda-ai-openapi.yml
  - https://www.fodda.ai/llms.txt
  - https://www.fodda.ai/llms-full.txt
  - live 402 on api.fodda.ai
  surfaces:
  - REST
  type: http
- description: 'Enterprise SSO via OIDC: Authorization: Bearer <jwt>. Issuer https://clerk.fodda.ai (Clerk-delegated; RS256, claims incl. email, org_id). Named in llms.txt/agents.txt and the legacy agent document; the REST OpenAPI does not declare it.'
  name: oidc
  openIdConnectUrl: https://clerk.fodda.ai/.well-known/openid-configuration
  sources:
  - https://www.fodda.ai/llms.txt
  - https://www.fodda.ai/agents.txt
  - well-known/fodda-ai-clerk-openid-configuration.json
  - a2a/fodda-ai-agent-legacy.json
  surfaces:
  - REST (enterprise)
  - MCP
  type: openIdConnect
- description: OAuth 2.1 for the MCP server, discovered per RFC 9728 from the 401 challenge. Resource metadata on mcp.fodda.ai names authorization server https://clerk.fodda.ai; dynamic client registration is supported.
  flows:
  - authorization_endpoint: https://clerk.fodda.ai/oauth/authorize
    authorization_server: https://clerk.fodda.ai
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    introspection_endpoint: https://clerk.fodda.ai/oauth/token_info
    pkce: S256
    registration_endpoint: https://clerk.fodda.ai/oauth/register
    revocation_endpoint: https://clerk.fodda.ai/oauth/token/revoke
    scopes:
    - openid
    - profile
    - email
    - public_metadata
    - private_metadata
    - offline_access
    - user:org:read
    token_endpoint: https://clerk.fodda.ai/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
    userinfo_endpoint: https://clerk.fodda.ai/oauth/userinfo
  - device_authorization_endpoint: https://clerk.fodda.ai/oauth/device_authorization
    flow: deviceCode
    grant_types:
    - urn:ietf:params:oauth:grant-type:device_code
  name: oauth2
  protected_resources:
  - metadata: well-known/fodda-ai-mcp-oauth-protected-resource.json
    resource: https://mcp.fodda.ai
  - metadata: well-known/fodda-ai-mcp-oauth-protected-resource-mcp.json
    resource: https://mcp.fodda.ai/mcp
  - metadata: well-known/fodda-ai-mcp-oauth-protected-resource-copilot.json
    resource: https://mcp.fodda.ai/copilot
  - bearer_methods_supported:
    - header
    metadata: well-known/fodda-ai-www-oauth-protected-resource.json
    resource: https://mcp.fodda.ai/mcp (as published on www)
    scopes_supported:
    - read
  sources:
  - well-known/fodda-ai-clerk-oauth-authorization-server.json
  - live WWW-Authenticate on POST https://mcp.fodda.ai/mcp
  surfaces:
  - MCP
  type: oauth2
- description: 'MCP-only: https://mcp.fodda.ai/c/<token> from app.fodda.ai -> Account -> MCP Integration, pasted into Claude/ChatGPT connectors with OAuth client fields left blank. Legacy ?api_key= / ?user_id= URLs are deprecated and return 401.'
  in: path
  name: personalConnectionUrl
  parameter: token
  sources:
  - fodda-mcp README
  - https://www.fodda.ai/platform-integration-anthropic-claude
  surfaces:
  - MCP
  type: apiKey
slug: fodda-ai-authentication
source_filename: fodda-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/fodda-ai-openapi.yml + openapi/fodda-ai-context-delivery-openapi.yml (securitySchemes) + https://www.fodda.ai/llms.txt\n  + https://www.fodda.ai/llms-full.txt (RULE AuthenticationRules) + well-known/fodda-ai-clerk-openid-configuration.json\n  + well-known/fodda-ai-clerk-oauth-authorization-server.json + well-known/fodda-ai-mcp-oauth-protected-resource*.json\n  + a2a/fodda-ai-agent-legacy.json securitySchemes + live 401/402 challenges (2026-09-19)\ndocs: https://www.fodda.ai/api\nsummary:\n  types:\n  - apiKey\n  - http\n  - openIdConnect\n  - oauth2\n  api_key_in:\n  - header\n  - query (deprecated for MCP URLs)\n  oauth2_flows:\n  - authorizationCode (PKCE S256)\n  - deviceCode\n  - refresh_token\n  rails: 'Three rails meter one unit: account API key (free tier), Stripe Shared Payment Token via HTTP 402 (no\n    account), enterprise OIDC JWT. The MCP server adds OAuth 2.1 delegated to clerk.fodda.ai and personal connection\n\
  \    URLs.'\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Required for all endpoints unless marked public. Issued at app.fodda.ai (Account); free tier $50\n    of API calls / 100 calls per month with a card on file, then $0.50 per call. Self-serve key rotation at app.fodda.ai\n    (compliance dossier). Copilot Studio guide also accepts Authorization: Bearer <api key>. Autonomous provisioning:\n    POST /api/account/b2b-provision (named on /agents; not in the OpenAPI).'\n  sources:\n  - openapi/fodda-ai-openapi.yml\n  - openapi/fodda-ai-context-delivery-openapi.yml\n  - https://www.fodda.ai/llms.txt\n  - https://www.fodda.ai/agents\n  surfaces:\n  - REST\n  - MCP (header or personal URL)\n- name: stripeSPT\n  type: http\n  scheme: bearer\n  bearer_format: spt_... (Stripe Shared Payment Token)\n  description: 'Machine Payments Protocol: call any endpoint with no credentials, receive HTTP 402 with the exact\n    price (WWW-Authenticate: stripe-spt\
  \ amount=<cents> currency=usd), obtain an SPT from Stripe Link, retry with\n    Authorization: Bearer spt_xxx or X-Stripe-SPT: spt_xxx. Price = API-call count × $0.50. Direct REST API only\n    (not MCP). Validate with GET /v1/spt/validate.'\n  sources:\n  - openapi/fodda-ai-openapi.yml\n  - https://www.fodda.ai/llms.txt\n  - https://www.fodda.ai/llms-full.txt\n  - live 402 on api.fodda.ai\n  surfaces:\n  - REST\n- name: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://clerk.fodda.ai/.well-known/openid-configuration\n  description: 'Enterprise SSO via OIDC: Authorization: Bearer <jwt>. Issuer https://clerk.fodda.ai (Clerk-delegated;\n    RS256, claims incl. email, org_id). Named in llms.txt/agents.txt and the legacy agent document; the REST OpenAPI\n    does not declare it.'\n  sources:\n  - https://www.fodda.ai/llms.txt\n  - https://www.fodda.ai/agents.txt\n  - well-known/fodda-ai-clerk-openid-configuration.json\n  - a2a/fodda-ai-agent-legacy.json\n  surfaces:\n  - REST (enterprise)\n\
  \  - MCP\n- name: oauth2\n  type: oauth2\n  description: OAuth 2.1 for the MCP server, discovered per RFC 9728 from the 401 challenge. Resource metadata on\n    mcp.fodda.ai names authorization server https://clerk.fodda.ai; dynamic client registration is supported.\n  flows:\n  - flow: authorizationCode\n    authorization_server: https://clerk.fodda.ai\n    authorization_endpoint: https://clerk.fodda.ai/oauth/authorize\n    token_endpoint: https://clerk.fodda.ai/oauth/token\n    registration_endpoint: https://clerk.fodda.ai/oauth/register\n    revocation_endpoint: https://clerk.fodda.ai/oauth/token/revoke\n    introspection_endpoint: https://clerk.fodda.ai/oauth/token_info\n    userinfo_endpoint: https://clerk.fodda.ai/oauth/userinfo\n    pkce: S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n    scopes:\n    - openid\n    - profile\n    - email\n    - public_metadata\n    - private_metadata\n    - offline_access\n    - user:org:read\n    token_endpoint_auth_methods:\n\
  \    - client_secret_basic\n    - client_secret_post\n    - none\n  - flow: deviceCode\n    device_authorization_endpoint: https://clerk.fodda.ai/oauth/device_authorization\n    grant_types:\n    - urn:ietf:params:oauth:grant-type:device_code\n  protected_resources:\n  - resource: https://mcp.fodda.ai\n    metadata: well-known/fodda-ai-mcp-oauth-protected-resource.json\n  - resource: https://mcp.fodda.ai/mcp\n    metadata: well-known/fodda-ai-mcp-oauth-protected-resource-mcp.json\n  - resource: https://mcp.fodda.ai/copilot\n    metadata: well-known/fodda-ai-mcp-oauth-protected-resource-copilot.json\n  - resource: https://mcp.fodda.ai/mcp (as published on www)\n    metadata: well-known/fodda-ai-www-oauth-protected-resource.json\n    scopes_supported:\n    - read\n    bearer_methods_supported:\n    - header\n  sources:\n  - well-known/fodda-ai-clerk-oauth-authorization-server.json\n  - live WWW-Authenticate on POST https://mcp.fodda.ai/mcp\n  surfaces:\n  - MCP\n- name: personalConnectionUrl\n\
  \  type: apiKey\n  in: path\n  parameter: token\n  description: 'MCP-only: https://mcp.fodda.ai/c/<token> from app.fodda.ai -> Account -> MCP Integration, pasted\n    into Claude/ChatGPT connectors with OAuth client fields left blank. Legacy ?api_key= / ?user_id= URLs are deprecated\n    and return 401.'\n  sources:\n  - fodda-mcp README\n  - https://www.fodda.ai/platform-integration-anthropic-claude\n  surfaces:\n  - MCP\npublic_tier:\n  no_credential_required:\n  - GET /v1/health\n  - GET /v1/research/pricing\n  - GET /v1/offerings\n  - GET /v1/research/offerings\n  - GET /v1/graphs/catalog\n  - GET /v1/analysts\n  - GET /v1/graph-slice\n  - GET /v1/catalog.okf\n  - GET /openapi.json\n  note: Verified live 2026-09-19. The spec marks POST /v1/psfk/overview public but it answered 402 unauthenticated.\nchallenges_observed:\n- surface: api.fodda.ai secured operation\n  status: 402\n  www_authenticate: stripe-spt amount=50 currency=usd\n- surface: mcp.fodda.ai /mcp, /copilot, /sse\n  status:\
  \ 401\n  www_authenticate: Bearer resource_metadata=\"https://mcp.fodda.ai/.well-known/oauth-protected-resource/mcp\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fodda-ai/refs/heads/main/authentication/fodda-ai-authentication.yml
summary_line: apiKey/http/openIdConnect/oauth2 · 5 schemes
tags:
- Market Intelligence
- Trend Research
- Knowledge Graph
- Consumer Insights
- Earnings Intelligence
- Brand Intelligence
- Research
- Institutional Data
- MCP
- A2A
- agent-native
- Machine Payments
- Company
---
