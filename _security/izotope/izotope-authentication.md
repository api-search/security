---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Izotope Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: iZotope secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: iZotope
provider_slug: izotope
scheme_count: 1
schemes:
- authorization_endpoint: https://account.izotope.com/authentication/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.izotope.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/73782919339
  jwks_uri: https://account.izotope.com/authentication/.well-known/jwks.json
  name: izotope-customer-accounts
  openIdConnectUrl: https://www.izotope.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/izotope-openid-configuration.json
  - well-known/izotope-oauth-authorization-server.json
  subject_types_supported:
  - public
  token_endpoint: https://account.izotope.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: izotope-authentication
source_filename: izotope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://www.izotope.com/.well-known/openid-configuration\ndocs: https://www.izotope.com/llms.txt\nnote: >-\n  iZotope publishes no OpenAPI, so this profile is not derived from\n  securitySchemes. It is read from the live OIDC / OAuth discovery documents\n  iZotope serves on its own hosts (www.izotope.com and account.izotope.com),\n  plus the anonymous-access behaviour observed on the UCP MCP endpoint.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces:\n    - https://www.izotope.com/api/ucp/mcp (tools/list and catalog reads require no token)\n    - https://www.izotope.com/products.json (public storefront product JSON)\nschemes:\n  - name: izotope-customer-accounts\n    type: openIdConnect\n    openIdConnectUrl: https://www.izotope.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/73782919339\n    authorization_endpoint: https://account.izotope.com/authentication/oauth/authorize\n\
  \    token_endpoint: https://account.izotope.com/authentication/oauth/token\n    end_session_endpoint: https://account.izotope.com/authentication/logout\n    jwks_uri: https://account.izotope.com/authentication/.well-known/jwks.json\n    response_types_supported: [code]\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    code_challenge_methods_supported: [S256]\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n    scopes_supported:\n      - openid\n      - email\n      - 'customer-account-api:full'\n      - 'customer-account-mcp-api:full'\n    sources:\n      - well-known/izotope-openid-configuration.json\n      - well-known/izotope-oauth-authorization-server.json\nprotected_resource:\n  spec: RFC 9728 OAuth 2.0\
  \ Protected Resource Metadata\n  url: https://www.izotope.com/.well-known/oauth-protected-resource\n  resource: https://www.izotope.com\n  authorization_servers:\n    - https://account.izotope.com\n    - https://shopify.com/authentication/73782919339\n  source: well-known/izotope-oauth-protected-resource.json\nagent_identity:\n  mechanism: UCP agent profile\n  parameter: meta.ucp-agent.profile\n  required: true\n  description: >-\n    The MCP tools do not take a bearer token for read operations; instead every\n    tool call must carry a `meta.ucp-agent.profile` URI identifying the calling\n    agent. Omitting it returns JSON-RPC error -32001 (invalid_profile_url).\n    Buyer payment is authorized out-of-band and requires contemporaneous human\n    approval per iZotope's own llms.txt.\nx-evidence:\n  fetched: '2026-08-12'\n  urls:\n    - {url: 'https://www.izotope.com/.well-known/openid-configuration', status: 200}\n    - {url: 'https://www.izotope.com/.well-known/oauth-protected-resource',\
  \ status: 200}\n    - {url: 'https://account.izotope.com/authentication/.well-known/jwks.json', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/izotope/refs/heads/main/authentication/izotope-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Audio
- Audio Software
- Music Production
- Mixing
- Mastering
- Audio Restoration
- Audio Repair
- Post Production
- Plugins
- VST
- AudioUnit
- AAX
- DSP
- AI Audio
- Machine Learning Audio
- Vocal Processing
- Agent Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Ecommerce
- Boris FX
---
