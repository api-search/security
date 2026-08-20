---
api_key_in: []
auth_types:
- none
- openIdConnect
- oauth2
- agentProfile
description: Black Buffalo publishes no OpenAPI, so this profile is built from live discovery documents and observed responses rather than derived securitySchemes. Four distinct auth postures were observed on 2026-08-07 — and notably, THREE of the four machine surfaces answered with no credential at all.
kind: authentication
layout: security
method: probed
name: Black Buffalo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Black Buffalo secures its APIs with none, openIdConnect, oauth2, and agentProfile across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Black Buffalo
provider_slug: black-buffalo
scheme_count: 7
schemes:
- name: anonymous-storefront-graphql
  observed: Full GraphQL introspection succeeded with no X-Shopify-Storefront-Access-Token header, on three separate API versions. Cost limiting is signalled via extensions.cost on every response rather than by an auth challenge.
  sources:
  - graphql/black-buffalo-graphql.yml
  surface: https://blackbuffalo.com/api/2026-04/graphql.json
  type: none
- name: anonymous-storefront-mcp
  observed: An unauthenticated JSON-RPC tools/list returned HTTP 200 with five tools and their input schemas. No Authorization header, API key or Storefront token required.
  sources:
  - mcp/black-buffalo-mcp.yml
  surface: https://blackbuffalo.com/api/mcp
  type: none
- name: anonymous-ucp-mcp-discovery
  observed: An unauthenticated tools/list returned HTTP 200 with all thirteen commerce tools, including complete_checkout. Discovery of the commerce surface requires no credential.
  sources:
  - mcp/black-buffalo-mcp.yml
  surface: https://blackbuffalo.com/api/ucp/mcp
  type: none
- mechanism: Every one of the thirteen UCP tools declares meta["ucp-agent"]["profile"] — a resolvable agent profile URI — as a REQUIRED input property. resources/list and prompts/list already fail without it, returning JSON-RPC error -32001 "UCP discovery failed" with code invalid_profile_url ("Missing profile uri").
  name: ucp-agent-profile
  note: This is agent IDENTITY, not shopper authorization. Payment authorization is separate and, per the provider's own robots.txt, must be approved by a human at the time of purchase.
  observed: 'Confirmed on 2026-08-07: tools/list is open, but the agent-identity requirement is enforced on invocation and on the resource/prompt methods.'
  sources:
  - mcp/black-buffalo-ucp-mcp-tools.json
  - well-known/black-buffalo-ucp.json
  spec: https://ucp.dev/2026-04-08/specification/overview/
  surface: https://blackbuffalo.com/api/ucp/mcp
  type: agentProfile
- authorizationUrl: https://shopify.com/authentication/22588521/oauth/authorize
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  end_session_endpoint: https://shopify.com/authentication/22588521/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/22588521
  jwks_uri: https://shopify.com/authentication/22588521/.well-known/jwks.json
  name: shopify-customer-accounts
  openIdConnectUrl: https://blackbuffalo.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/black-buffalo-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/22588521/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- name: shopify-customer-accounts-oauth2
  note: The same authorization server also publishes RFC 8414 metadata at /.well-known/oauth-authorization-server (byte-identical document), so the surface is usable as plain OAuth 2.0 as well as OIDC.
  sources:
  - well-known/black-buffalo-oauth-authorization-server.json
  type: oauth2
- header: X-Shopify-Customer-Access-Token
  mechanism: The Storefront GraphQL schema itself carries a legacy shopper-token flow — customerAccessTokenCreate / customerAccessTokenRenew / customerAccessTokenDelete mutations, consumed by the customer query and the customer* mutations. Distinct from the OIDC customer-accounts flow above.
  name: storefront-customer-access-token
  scheme: bearer
  sources:
  - graphql/black-buffalo-storefront.graphql
  surface: https://blackbuffalo.com/api/2026-04/graphql.json
  type: http
slug: black-buffalo-authentication
source_filename: black-buffalo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://blackbuffalo.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  Black Buffalo publishes no OpenAPI, so this profile is built from live discovery\n  documents and observed responses rather than derived securitySchemes. Four distinct\n  auth postures were observed on 2026-08-07 — and notably, THREE of the four machine\n  surfaces answered with no credential at all.\nsummary:\n  types: [none, openIdConnect, oauth2, agentProfile]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\nschemes:\n- name: anonymous-storefront-graphql\n  type: none\n  surface: https://blackbuffalo.com/api/2026-04/graphql.json\n  observed: >-\n    Full GraphQL introspection succeeded with no X-Shopify-Storefront-Access-Token\n    header, on three separate API versions. Cost limiting is signalled via\n    extensions.cost on every response rather than by an auth challenge.\n\
  \  sources: [graphql/black-buffalo-graphql.yml]\n- name: anonymous-storefront-mcp\n  type: none\n  surface: https://blackbuffalo.com/api/mcp\n  observed: >-\n    An unauthenticated JSON-RPC tools/list returned HTTP 200 with five tools and their\n    input schemas. No Authorization header, API key or Storefront token required.\n  sources: [mcp/black-buffalo-mcp.yml]\n- name: anonymous-ucp-mcp-discovery\n  type: none\n  surface: https://blackbuffalo.com/api/ucp/mcp\n  observed: >-\n    An unauthenticated tools/list returned HTTP 200 with all thirteen commerce tools,\n    including complete_checkout. Discovery of the commerce surface requires no\n    credential.\n  sources: [mcp/black-buffalo-mcp.yml]\n- name: ucp-agent-profile\n  type: agentProfile\n  surface: https://blackbuffalo.com/api/ucp/mcp\n  mechanism: >-\n    Every one of the thirteen UCP tools declares meta[\"ucp-agent\"][\"profile\"] — a\n    resolvable agent profile URI — as a REQUIRED input property. resources/list and\n   \
  \ prompts/list already fail without it, returning JSON-RPC error -32001\n    \"UCP discovery failed\" with code invalid_profile_url (\"Missing profile uri\").\n  observed: >-\n    Confirmed on 2026-08-07: tools/list is open, but the agent-identity requirement is\n    enforced on invocation and on the resource/prompt methods.\n  spec: https://ucp.dev/2026-04-08/specification/overview/\n  note: >-\n    This is agent IDENTITY, not shopper authorization. Payment authorization is separate\n    and, per the provider's own robots.txt, must be approved by a human at the time of\n    purchase.\n  sources: [mcp/black-buffalo-ucp-mcp-tools.json, well-known/black-buffalo-ucp.json]\n- name: shopify-customer-accounts\n  type: openIdConnect\n  openIdConnectUrl: https://blackbuffalo.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/22588521\n  authorizationUrl: https://shopify.com/authentication/22588521/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/22588521/oauth/token\n\
  \  end_session_endpoint: https://shopify.com/authentication/22588521/logout\n  jwks_uri: https://shopify.com/authentication/22588521/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic]\n  pkce: [S256]\n  id_token_signing_alg: [RS256]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/black-buffalo-openid-configuration.json]\n- name: shopify-customer-accounts-oauth2\n  type: oauth2\n  note: >-\n    The same authorization server also publishes RFC 8414 metadata at\n    /.well-known/oauth-authorization-server (byte-identical document), so the surface is\n    usable as plain OAuth 2.0 as well as OIDC.\n  sources: [well-known/black-buffalo-oauth-authorization-server.json]\n- name: storefront-customer-access-token\n\
  \  type: http\n  scheme: bearer\n  surface: https://blackbuffalo.com/api/2026-04/graphql.json\n  header: X-Shopify-Customer-Access-Token\n  mechanism: >-\n    The Storefront GraphQL schema itself carries a legacy shopper-token flow —\n    customerAccessTokenCreate / customerAccessTokenRenew / customerAccessTokenDelete\n    mutations, consumed by the customer query and the customer* mutations. Distinct from\n    the OIDC customer-accounts flow above.\n  sources: [graphql/black-buffalo-storefront.graphql]\nage_gating:\n  present: true\n  surface: human web only\n  detail: >-\n    Black Buffalo sells a nicotine product restricted to adults 21+ and runs age\n    verification on the storefront (/pages/verify-age, /pages/verify-age-ca). NO age or\n    eligibility assertion is required, offered, or checked on any of the machine\n    surfaces — the anonymous GraphQL, Storefront MCP and UCP MCP endpoints all answered\n    without one. /agents.md states the restriction in prose and instructs agents\
  \ not to\n    recommend the products to anyone under 21, but that instruction is unenforced at the\n    protocol layer.\n  note: >-\n    Recorded as an observed fact about the auth surface, not as a compliance finding.\nx-evidence:\n- fetched: '2026-08-07'\n  url: https://blackbuffalo.com/.well-known/openid-configuration\n  http_status: 200\n- fetched: '2026-08-07'\n  url: https://blackbuffalo.com/api/2026-04/graphql.json\n  http_status: 200\n  note: anonymous introspection\n- fetched: '2026-08-07'\n  url: https://blackbuffalo.com/api/ucp/mcp\n  http_status: 200\n  note: anonymous tools/list; resources/list rejected with -32001 invalid_profile_url\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-buffalo/refs/heads/main/authentication/black-buffalo-authentication.yml
summary_line: none/openIdConnect/oauth2/agentProfile · 7 schemes
tags:
- Company
- Consumer Packaged Goods
- Nicotine Pouches
- Smokeless Tobacco Alternative
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
---
