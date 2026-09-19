---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Hni Authentication
name_suffix: Authentication
oauth_flows: []
overview: HNI Corporation declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: HNI Corporation
provider_slug: hni
scheme_count: 4
schemes:
- applies_to: 'https://hearthnhome.com/api/ucp/mcp (method: tools/list)'
  description: Tool DISCOVERY is anonymous. tools/list returned HTTP 200 with the full 13-tool manifest and complete inputSchemas, with no Authorization header.
  evidence:
    http_status: 200
    probed: '2026-09-13'
    url: https://hearthnhome.com/api/ucp/mcp
  id: anonymous-discovery
  type: none
- applies_to: 'https://hearthnhome.com/api/ucp/mcp (method: tools/call)'
  description: Tool EXECUTION requires `meta.ucp-agent.profile`, an absolute https URI the server fetches over HTTP before dispatch. Omitting it returns JSON-RPC -32001 invalid_profile_url; supplying an unreachable URI returns -32001 profile_unreachable. This is an identity assertion the agent must actually publish, not a bearer secret.
  evidence:
    http_status: 200
    observed_error: '{"code":-32001,"message":"UCP discovery failed","data":{"code":"invalid_profile_url",...}}'
    probed: '2026-09-13'
    url: https://hearthnhome.com/api/ucp/mcp
  id: ucp-agent-profile
  type: agentIdentity
- applies_to: 'https://hearthnhome.com/api/ucp/mcp (method: tools/call)'
  bearerFormat: JWT
  description: Beyond the agent profile, tools/call demands a valid Shopify agent JWT. An unauthenticated call returns JSON-RPC -32000 "AuthenticationRequired" with the message "A valid JWT is required to call <tool>. See https://shopify.dev/docs/agents/get-started/authentication". The endpoint is therefore OPEN TO DISCOVERY BUT CLOSED TO EXECUTION — a distinction the llms.txt does not make.
  docs: https://shopify.dev/docs/agents/get-started/authentication
  evidence:
    http_status: 200
    probed: '2026-09-13'
    url: https://hearthnhome.com/api/ucp/mcp
  id: shopify-agent-jwt
  scheme: bearer
  type: http
- applies_to: customer account data on hearthnhome.com
  authorization_endpoint: https://shopify.com/authentication/67598516522/oauth/authorize
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
  description: Shopify-operated customer account authentication. The authorization server lives on shopify.com, not on an HNI host; hearthnhome.com publishes the discovery document and the RFC 9728 protected resource metadata that points at it.
  end_session_endpoint: https://shopify.com/authentication/67598516522/logout
  evidence:
    http_status: 200
    probed: '2026-09-13'
    url: https://hearthnhome.com/.well-known/openid-configuration
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/67598516522
  jwks_uri: https://shopify.com/authentication/67598516522/.well-known/jwks.json
  openIdConnectUrl: https://hearthnhome.com/.well-known/openid-configuration
  pkce:
    required_methods:
    - S256
  response_types:
  - code
  subject_types:
  - public
  token_endpoint: https://shopify.com/authentication/67598516522/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: hni-authentication
source_filename: hni-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://hearthnhome.com/.well-known/openid-configuration\ndocs: https://hearthnhome.com/agents.md\nnote: >-\n  HNI Corporation publishes no developer portal and no OpenAPI, so no securityScheme could be derived.\n  This profile is built entirely from discovery documents fetched live from hearthnhome.com on\n  2026-09-13. Two distinct postures coexist on the same host.\nschemes:\n  - id: anonymous-discovery\n    type: none\n    applies_to: 'https://hearthnhome.com/api/ucp/mcp (method: tools/list)'\n    description: >-\n      Tool DISCOVERY is anonymous. tools/list returned HTTP 200 with the full 13-tool manifest and\n      complete inputSchemas, with no Authorization header.\n    evidence:\n      url: https://hearthnhome.com/api/ucp/mcp\n      http_status: 200\n      probed: '2026-09-13'\n  - id: ucp-agent-profile\n    type: agentIdentity\n    applies_to: 'https://hearthnhome.com/api/ucp/mcp (method: tools/call)'\n    description:\
  \ >-\n      Tool EXECUTION requires `meta.ucp-agent.profile`, an absolute https URI the server fetches over\n      HTTP before dispatch. Omitting it returns JSON-RPC -32001 invalid_profile_url; supplying an\n      unreachable URI returns -32001 profile_unreachable. This is an identity assertion the agent must\n      actually publish, not a bearer secret.\n    evidence:\n      url: https://hearthnhome.com/api/ucp/mcp\n      http_status: 200\n      probed: '2026-09-13'\n      observed_error: '{\"code\":-32001,\"message\":\"UCP discovery failed\",\"data\":{\"code\":\"invalid_profile_url\",...}}'\n  - id: shopify-agent-jwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to: 'https://hearthnhome.com/api/ucp/mcp (method: tools/call)'\n    description: >-\n      Beyond the agent profile, tools/call demands a valid Shopify agent JWT. An unauthenticated call\n      returns JSON-RPC -32000 \"AuthenticationRequired\" with the message \"A valid JWT is required to call\n   \
  \   <tool>. See https://shopify.dev/docs/agents/get-started/authentication\". The endpoint is therefore\n      OPEN TO DISCOVERY BUT CLOSED TO EXECUTION — a distinction the llms.txt does not make.\n    docs: https://shopify.dev/docs/agents/get-started/authentication\n    evidence:\n      url: https://hearthnhome.com/api/ucp/mcp\n      http_status: 200\n      probed: '2026-09-13'\n  - id: shopify-customer-account-oidc\n    type: openIdConnect\n    applies_to: customer account data on hearthnhome.com\n    openIdConnectUrl: https://hearthnhome.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/67598516522\n    authorization_endpoint: https://shopify.com/authentication/67598516522/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/67598516522/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/67598516522/logout\n    jwks_uri: https://shopify.com/authentication/67598516522/.well-known/jwks.json\n    grant_types:\n\
  \      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    response_types:\n      - code\n    pkce:\n      required_methods:\n        - S256\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n    id_token_signing_alg:\n      - RS256\n    claims:\n      - iss\n      - sub\n      - aud\n      - exp\n      - iat\n      - nonce\n      - sid\n      - email\n      - email_verified\n    subject_types:\n      - public\n    description: >-\n      Shopify-operated customer account authentication. The authorization server lives on shopify.com,\n      not on an HNI host; hearthnhome.com publishes the discovery document and the RFC 9728 protected\n      resource metadata that points at it.\n    evidence:\n      url: https://hearthnhome.com/.well-known/openid-configuration\n      http_status: 200\n      probed: '2026-09-13'\nprotected_resource_metadata:\n  present: true\n  url: https://hearthnhome.com/.well-known/oauth-protected-resource\n\
  \  resource: https://hearthnhome.com\n  authorization_servers:\n    - https://shopify.com/authentication/67598516522\n  bearer_methods_supported:\n    - header\n  rfc: RFC 9728\ndynamic_client_registration:\n  present: false\n  note: No registration_endpoint is advertised in the authorization server metadata.\ngaps:\n  - No authentication documentation exists on any HNI Corporation host; the only auth surface is the\n    Shopify platform discovery document on the storefront.\n  - www.hnicorp.com serves no /.well-known/security.txt and no developer or auth documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hni/refs/heads/main/authentication/hni-authentication.yml
summary_line: 4 schemes
tags:
- Fortune 1000
- Manufacturing
- Office Furniture
- Workplace
- Building Products
- Hearth
- Retail
- E-Commerce
- Agentic Commerce
- MCP
---
