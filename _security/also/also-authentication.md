---
api_key_in:
- header
api_specs:
- filename: also-storefront-json-openapi.yml
  format: yaml
  label: ALSO Storefront JSON API
  slug: also-storefront-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-storefront-json-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Also Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Also secures its APIs with none, oauth2, openIdConnect, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Also
provider_slug: also
scheme_count: 4
schemes:
- applies_to:
  - openapi/also-storefront-json-openapi.yml
  - graphql/also-storefront-2026-07.graphql
  description: Read-only product, collection, cart and search access requires no credential. Storefront GraphQL introspection and queries were confirmed open.
  evidence:
    http_status: 200
    probe: full __schema introspection with no X-Shopify-Storefront-Access-Token
    url: https://ridealso.com/api/2026-07/graphql.json
  name: anonymous-storefront
  type: none
- authorization_endpoint: https://shopify.com/authentication/74758783200/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/74758783200/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/74758783200
  jwks_uri: https://shopify.com/authentication/74758783200/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://ridealso.com/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/also-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/74758783200/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- authorization_endpoint: https://idp.ridealso.com/oauth2/authorize
  description: ALSO runs its own branded identity provider at idp.ridealso.com (AWS Cognito hosted UI) for the Continue with Google and Continue with Apple buttons on the storefront account login. Discovery documents are not served at the custom domain; the authorize endpoint and requested scopes were observed in the login links on ridealso.com.
  evidence:
    authorize_probe:
      http_status: 302
      url: https://idp.ridealso.com/oauth2/authorize
    discovery_probe:
      http_status: 404
      url: https://idp.ridealso.com/.well-known/openid-configuration
    source: https://ridealso.com/ (rendered login links)
  flows:
  - flow: authorizationCode
    redirect_uri: https://ridealso.com/apps/tools/auth/callback
    scopes:
    - openid
    - email
    - profile
  identity_providers:
  - Google
  - SignInWithApple
  logout_endpoint: https://idp.ridealso.com/logout
  name: also-idp-cognito
  token_endpoint: https://idp.ridealso.com/oauth2/token
  type: oauth2
  userinfo_endpoint: https://idp.ridealso.com/oauth2/userInfo
- applies_to:
  - mcp/also-mcp.yml
  description: Every call to the UCP MCP endpoint must carry `meta.ucp-agent.profile` (HTTP `UCP-Agent` header), a URI resolving to the calling platform's own UCP profile document. It is an agent identity assertion rather than a secret. Omitting it returns JSON-RPC error -32001 invalid_profile_url with HTTP 422.
  evidence:
    http_status: 422
    schema: https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json#/components/schemas/meta
    url: https://ridealso.com/api/ucp/mcp
  in: header
  name: ucp-agent-profile
  parameter_name: UCP-Agent
  type: apiKey
slug: also-authentication
source_filename: also-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://ridealso.com/.well-known/openid-configuration\ndocs: https://ridealso.com/agents.md\nsummary:\n  types: [none, oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  note: The Storefront GraphQL API on ridealso.com answered a full introspection query\n    with NO access token on 2026-08-02, so the read surface is effectively anonymous.\n    OAuth2/OIDC covers customer accounts; the UCP MCP endpoint gates on an agent\n    profile URI rather than a bearer token.\nschemes:\n- name: anonymous-storefront\n  type: none\n  applies_to:\n  - openapi/also-storefront-json-openapi.yml\n  - graphql/also-storefront-2026-07.graphql\n  description: Read-only product, collection, cart and search access requires no\n    credential. Storefront GraphQL introspection and queries were confirmed open.\n  evidence:\n    url: https://ridealso.com/api/2026-07/graphql.json\n  \
  \  http_status: 200\n    probe: full __schema introspection with no X-Shopify-Storefront-Access-Token\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://ridealso.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/74758783200\n  authorization_endpoint: https://shopify.com/authentication/74758783200/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/74758783200/oauth/token\n  jwks_uri: https://shopify.com/authentication/74758783200/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/74758783200/logout\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic]\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [RS256]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/also-openid-configuration.json]\n\
  - name: also-idp-cognito\n  type: oauth2\n  description: ALSO runs its own branded identity provider at idp.ridealso.com (AWS\n    Cognito hosted UI) for the Continue with Google and Continue with Apple buttons\n    on the storefront account login. Discovery documents are not served at the custom\n    domain; the authorize endpoint and requested scopes were observed in the login\n    links on ridealso.com.\n  authorization_endpoint: https://idp.ridealso.com/oauth2/authorize\n  token_endpoint: https://idp.ridealso.com/oauth2/token\n  userinfo_endpoint: https://idp.ridealso.com/oauth2/userInfo\n  logout_endpoint: https://idp.ridealso.com/logout\n  flows:\n  - flow: authorizationCode\n    scopes: [openid, email, profile]\n    redirect_uri: https://ridealso.com/apps/tools/auth/callback\n  identity_providers: [Google, SignInWithApple]\n  evidence:\n    source: https://ridealso.com/ (rendered login links)\n    authorize_probe: {url: 'https://idp.ridealso.com/oauth2/authorize', http_status: 302}\n\
  \    discovery_probe: {url: 'https://idp.ridealso.com/.well-known/openid-configuration',\n      http_status: 404}\n- name: ucp-agent-profile\n  type: apiKey\n  in: header\n  parameter_name: UCP-Agent\n  applies_to: [mcp/also-mcp.yml]\n  description: Every call to the UCP MCP endpoint must carry `meta.ucp-agent.profile`\n    (HTTP `UCP-Agent` header), a URI resolving to the calling platform's own UCP\n    profile document. It is an agent identity assertion rather than a secret. Omitting\n    it returns JSON-RPC error -32001 invalid_profile_url with HTTP 422.\n  evidence:\n    url: https://ridealso.com/api/ucp/mcp\n    http_status: 422\n    schema: https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json#/components/schemas/meta\nbuyer_consent:\n  required: true\n  statement: Checkout requires human approval. Agents must not complete payment without\n    explicit buyer consent.\n  source: https://ridealso.com/agents.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/authentication/also-authentication.yml
summary_line: none/oauth2/openIdConnect/apiKey · 4 schemes
tags:
- Company
- Micromobility
- Electric Vehicles
- Transportation
- E-Commerce
- Consumer Hardware
- Agentic Commerce
- Logistics
- Delivery
---
