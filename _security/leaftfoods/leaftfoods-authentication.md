---
api_key_in: []
auth_types: []
description: The Leaft Foods storefront exposes three distinct access modes — fully anonymous read-only storefront JSON, an agent-facing UCP/MCP endpoint whose write operations gate on buyer approval rather than an API key, and OpenID Connect customer-account login served by Shopify's hosted authorization server. There is no self-serve developer API-key programme published by Leaft Foods itself.
kind: authentication
layout: security
method: searched
name: Leaftfoods Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leaft Foods declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Leaft Foods
provider_slug: leaftfoods
scheme_count: 3
schemes:
- description: Read-only storefront data requires no authentication. Documented in the store's llms.txt as the path for agents that only need to read.
  endpoints:
  - GET /collections/all
  - GET /products/{handle}
  - GET /products/{handle}.json
  - GET /collections/{handle}
  - GET /collections/{handle}/products.json
  - GET /search?q={query}&type=product
  - GET /sitemap.xml
  - GET /cart.js
  id: anonymous_storefront
  type: none
  verified:
    date: '2026-07-19'
    note: GET /products.json?limit=3 returned HTTP 200 with an empty products array — reachable and unauthenticated, catalog not currently published through that path.
- description: The UCP MCP endpoint performs agent discovery rather than presenting a conventional API-key or bearer challenge. An unauthenticated tools/list is rejected with UCP error invalid_profile_url ("Missing profile uri"), meaning the calling agent must present a resolvable agent profile URI. Payment completion additionally requires contemporaneous human buyer approval, which is an authorization invariant of the protocol, not a credential.
  endpoint: https://www.leaftfoods.com/api/ucp/mcp
  flow: agent-profile
  id: ucp_mcp
  specification: https://ucp.dev/2026-04-08/specification/overview/
  type: openIdConnect
  verified:
    date: '2026-07-19'
    error_code: invalid_profile_url
    status: 422
- authorization_endpoint: https://shopify.com/authentication/95682920744/oauth/authorize
  authorization_server_metadata: https://www.leaftfoods.com/.well-known/oauth-authorization-server
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
  description: OpenID Connect / OAuth 2.0 for Shopify customer accounts, discovered from the storefront host but issued by Shopify on behalf of shop 95682920744.
  end_session_endpoint: https://shopify.com/authentication/95682920744/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: customer_account_oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/95682920744
  jwks_uri: https://shopify.com/authentication/95682920744/.well-known/jwks.json
  openid_configuration: https://www.leaftfoods.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  policy_uri: https://www.shopify.com/legal/privacy
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types:
  - public
  token_endpoint: https://shopify.com/authentication/95682920744/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  tos_uri: https://www.shopify.com/legal/terms
  type: openIdConnect
slug: leaftfoods-authentication
source_filename: leaftfoods-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.leaftfoods.com/.well-known/openid-configuration\ndocs: https://www.leaftfoods.com/llms.txt\nname: Leaft Foods Authentication Profile\ndescription: The Leaft Foods storefront exposes three distinct access modes — fully anonymous read-only\n  storefront JSON, an agent-facing UCP/MCP endpoint whose write operations gate on buyer approval rather\n  than an API key, and OpenID Connect customer-account login served by Shopify's hosted authorization\n  server. There is no self-serve developer API-key programme published by Leaft Foods itself.\nschemes:\n- id: anonymous_storefront\n  type: none\n  description: Read-only storefront data requires no authentication. Documented in the store's llms.txt as\n    the path for agents that only need to read.\n  endpoints:\n  - GET /collections/all\n  - GET /products/{handle}\n  - GET /products/{handle}.json\n  - GET /collections/{handle}\n  - GET /collections/{handle}/products.json\n\
  \  - GET /search?q={query}&type=product\n  - GET /sitemap.xml\n  - GET /cart.js\n  verified:\n    date: '2026-07-19'\n    note: GET /products.json?limit=3 returned HTTP 200 with an empty products array — reachable and\n      unauthenticated, catalog not currently published through that path.\n- id: ucp_mcp\n  type: openIdConnect\n  flow: agent-profile\n  description: The UCP MCP endpoint performs agent discovery rather than presenting a conventional API-key\n    or bearer challenge. An unauthenticated tools/list is rejected with UCP error invalid_profile_url\n    (\"Missing profile uri\"), meaning the calling agent must present a resolvable agent profile URI. Payment\n    completion additionally requires contemporaneous human buyer approval, which is an authorization\n    invariant of the protocol, not a credential.\n  endpoint: https://www.leaftfoods.com/api/ucp/mcp\n  specification: https://ucp.dev/2026-04-08/specification/overview/\n  verified:\n    date: '2026-07-19'\n    status: 422\n\
  \    error_code: invalid_profile_url\n- id: customer_account_oidc\n  type: openIdConnect\n  description: OpenID Connect / OAuth 2.0 for Shopify customer accounts, discovered from the storefront\n    host but issued by Shopify on behalf of shop 95682920744.\n  issuer: https://shopify.com/authentication/95682920744\n  openid_configuration: https://www.leaftfoods.com/.well-known/openid-configuration\n  authorization_server_metadata: https://www.leaftfoods.com/.well-known/oauth-authorization-server\n  authorization_endpoint: https://shopify.com/authentication/95682920744/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/95682920744/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/95682920744/logout\n  jwks_uri: https://shopify.com/authentication/95682920744/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  pkce:\n    supported: true\n  \
  \  code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  subject_types:\n  - public\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  policy_uri: https://www.shopify.com/legal/privacy\n  tos_uri: https://www.shopify.com/legal/terms\nnotes:\n- Authorization-code + PKCE (S256) is supported and is the correct public-client flow.\n- client_secret_basic is the only token-endpoint auth method advertised; there is no client_secret_post or\n  private_key_jwt.\n- The scope customer-account-mcp-api:full indicates a customer-account MCP surface distinct from the\n  storefront UCP MCP endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaftfoods/refs/heads/main/authentication/leaftfoods-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Food
- AgTech
- Alternative Protein
- Ingredients
- Pet Nutrition
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- New Zealand
---
