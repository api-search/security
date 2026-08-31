---
api_key_in: []
api_specs:
- filename: liquid-death-catalog-api-openapi.yml
  format: yaml
  label: Liquid Death Catalog API
  slug: liquid-death-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/openapi/liquid-death-catalog-api-openapi.yml
- filename: liquid-death-discovery-api-openapi.yml
  format: yaml
  label: Liquid Death Discovery API
  slug: liquid-death-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/openapi/liquid-death-discovery-api-openapi.yml
auth_types:
- none
- openIdConnect
- oauth2
- agentProfile
description: ''
kind: authentication
layout: security
method: probed
name: Liquid Death Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Liquid Death secures its APIs with none, openIdConnect, oauth2, and agentProfile across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Liquid Death
provider_slug: liquid-death
scheme_count: 4
schemes:
- applies_to: openapi/liquid-death-storefront-openapi.yml
  description: Every operation in the read-only storefront surface (/products/{handle}.json, /collections/{handle}/products.json, /search, /sitemap.xml, /agents.md, /llms.txt, /.well-known/ucp) returns 200 with no credential. Verified by live probe 2026-08-01.
  name: anonymous
  type: none
- applies_to: mcp/liquid-death-mcp.yml
  description: The UCP MCP endpoint identifies the calling platform, not a user. The caller supplies a URL to its own UCP profile document; the merchant fetches and validates it. An anonymous tools/list returns JSON-RPC error -32001 invalid_profile_url. This is an identity requirement rather than an authorization credential — it is what makes the agent attributable.
  format: uri
  in: header
  json_rpc_param: meta.ucp-agent.profile
  name: ucp-agent-profile
  parameter_name: UCP-Agent
  required: true
  source: https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json
  type: agentProfile
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  description: OpenID Connect provider for the Liquid Death customer account, hosted at account.liquiddeath.com and issued by Shopify on behalf of the store.
  endpoints:
    authorization: https://account.liquiddeath.com/authentication/oauth/authorize
    end_session: https://account.liquiddeath.com/authentication/logout
    jwks: https://account.liquiddeath.com/authentication/.well-known/jwks.json
    token: https://account.liquiddeath.com/authentication/oauth/token
  flows:
  - authorizationUrl: https://account.liquiddeath.com/authentication/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pkce: true
    tokenUrl: https://account.liquiddeath.com/authentication/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/7942897737
  name: customer-account-oidc
  openIdConnectUrl: https://liquiddeath.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: well-known/liquid-death-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- description: The same authorization server also publishes RFC 8414 OAuth 2.0 Authorization Server Metadata at /.well-known/oauth-authorization-server with an identical payload, so plain OAuth 2.0 clients can discover it without OIDC semantics.
  metadata_url: https://liquiddeath.com/.well-known/oauth-authorization-server
  name: customer-account-oauth2
  source: well-known/liquid-death-oauth-authorization-server.json
  type: oauth2
slug: liquid-death-authentication
source_filename: liquid-death-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://liquiddeath.com/.well-known/openid-configuration\ndocs: https://liquiddeath.com/agents.md\nsummary:\n  types: [none, openIdConnect, oauth2, agentProfile]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Liquid Death runs three distinct access modes. The read-only storefront JSON surface is fully\n    anonymous. The UCP MCP transport requires an agent identity (a resolvable UCP agent profile URL,\n    not a bearer credential). Customer-scoped operations use a Shopify-issued OpenID Connect provider\n    on the store's own account subdomain.\nschemes:\n  - name: anonymous\n    type: none\n    applies_to: openapi/liquid-death-storefront-openapi.yml\n    description: >-\n      Every operation in the read-only storefront surface (/products/{handle}.json,\n      /collections/{handle}/products.json, /search, /sitemap.xml, /agents.md, /llms.txt,\n      /.well-known/ucp) returns 200 with no credential. Verified\
  \ by live probe 2026-08-01.\n  - name: ucp-agent-profile\n    type: agentProfile\n    applies_to: mcp/liquid-death-mcp.yml\n    in: header\n    parameter_name: UCP-Agent\n    json_rpc_param: meta.ucp-agent.profile\n    format: uri\n    required: true\n    description: >-\n      The UCP MCP endpoint identifies the calling platform, not a user. The caller supplies a URL to its\n      own UCP profile document; the merchant fetches and validates it. An anonymous tools/list returns\n      JSON-RPC error -32001 invalid_profile_url. This is an identity requirement rather than an\n      authorization credential — it is what makes the agent attributable.\n    source: https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json\n  - name: customer-account-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://liquiddeath.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/7942897737\n    description: >-\n      OpenID Connect provider for the Liquid Death customer\
  \ account, hosted at\n      account.liquiddeath.com and issued by Shopify on behalf of the store.\n    endpoints:\n      authorization: https://account.liquiddeath.com/authentication/oauth/authorize\n      token: https://account.liquiddeath.com/authentication/oauth/token\n      end_session: https://account.liquiddeath.com/authentication/logout\n      jwks: https://account.liquiddeath.com/authentication/.well-known/jwks.json\n    flows:\n      - flow: authorizationCode\n        pkce: true\n        code_challenge_methods: [S256]\n        authorizationUrl: https://account.liquiddeath.com/authentication/oauth/authorize\n        tokenUrl: https://account.liquiddeath.com/authentication/oauth/token\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    response_types_supported: [code]\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported:\
  \ [public]\n    claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n    scopes_supported:\n      - openid\n      - email\n      - 'customer-account-api:full'\n      - 'customer-account-mcp-api:full'\n    source: well-known/liquid-death-openid-configuration.json\n  - name: customer-account-oauth2\n    type: oauth2\n    description: >-\n      The same authorization server also publishes RFC 8414 OAuth 2.0 Authorization Server Metadata at\n      /.well-known/oauth-authorization-server with an identical payload, so plain OAuth 2.0 clients can\n      discover it without OIDC semantics.\n    metadata_url: https://liquiddeath.com/.well-known/oauth-authorization-server\n    source: well-known/liquid-death-oauth-authorization-server.json\nobservations:\n  - >-\n    Publishing BOTH /.well-known/openid-configuration and /.well-known/oauth-authorization-server is\n    uncommon and materially improves discoverability for agent clients that only implement RFC 8414.\n  - >-\n\
  \    The customer-account-mcp-api:full scope indicates the identity provider is already wired for\n    MCP-mediated customer access, distinct from the anonymous UCP shopping transport.\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n    - {url: 'https://liquiddeath.com/.well-known/openid-configuration', http_status: 200}\n    - {url: 'https://liquiddeath.com/.well-known/oauth-authorization-server', http_status: 200}\n    - {url: 'https://account.liquiddeath.com/authentication/.well-known/jwks.json', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/authentication/liquid-death-authentication.yml
summary_line: none/openIdConnect/oauth2/agentProfile · 4 schemes
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Retail
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
