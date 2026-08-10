---
api_key_in: []
auth_types: []
description: 'SAMBAZON has no developer program and issues no API keys. Authentication on its public surface comes from two places: (1) nothing at all — the read-only Shopify storefront JSON endpoints and the discovery documents are unauthenticated; and (2) the Shopify customer-account OpenID Connect provider, whose metadata this origin publishes and whose authorization server is Shopify''s, not SAMBAZON''s. The UCP/MCP endpoint is a third case: it is not key- or token-gated but PROFILE-gated — it requires the calling agent to present a resolvable UCP agent profile URI before it will do anything.'
kind: authentication
layout: security
method: probed
name: Sambazon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sambazon declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Sambazon
provider_slug: sambazon
scheme_count: 3
schemes:
- applies_to:
  - https://www.sambazon.com/products.json
  - https://www.sambazon.com/products/{handle}.json
  - https://www.sambazon.com/collections/{handle}/products.json
  - https://www.sambazon.com/search/suggest.json
  - https://www.sambazon.com/.well-known/ucp
  - https://www.sambazon.com/llms.txt
  - https://www.sambazon.com/agents.md
  description: Read-only browsing requires no authentication. The store's own llms.txt documents these under the heading "Read-Only Browsing (No Authentication Required)". Verified with anonymous GETs returning 200 application/json.
  id: none
  type: none
- applies_to:
  - https://www.sambazon.com/api/ucp/mcp
  description: The UCP/MCP endpoint rejects anonymous JSON-RPC with error -32001 "UCP discovery failed" / data.code "invalid_profile_url" / "Missing profile uri". This is an agent-identity gate defined by the Universal Commerce Protocol rather than a conventional API credential — the caller must be a registered agent with a fetchable profile. The store publishes no instructions for obtaining one; agents.md simply says to call tools/list.
  id: ucp_agent_profile
  observed_http_status: 422
  spec: https://ucp.dev/2026-04-08/specification/overview/
  type: agent-identity
- authorization_endpoint: https://shopify.com/authentication/52008485056/oauth/authorize
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
  description: Shopify's customer-account identity provider, discoverable from this origin. Governs shopper login on www.sambazon.com/account/login and the customer-account API/MCP scopes. The authorization server and the login UI are Shopify's; SAMBAZON operates neither.
  end_session_endpoint: https://shopify.com/authentication/52008485056/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_account_oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/52008485056
  jwks_uri: https://shopify.com/authentication/52008485056/.well-known/jwks.json
  openIdConnectUrl: https://www.sambazon.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes: ../scopes/sambazon-scopes.yml
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/52008485056/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: sambazon-authentication
source_filename: sambazon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: >-\n  https://www.sambazon.com/.well-known/openid-configuration,\n  https://www.sambazon.com/.well-known/oauth-protected-resource,\n  https://www.sambazon.com/.well-known/ucp,\n  https://www.sambazon.com/agents.md\ndescription: >-\n  SAMBAZON has no developer program and issues no API keys. Authentication on\n  its public surface comes from two places: (1) nothing at all — the read-only\n  Shopify storefront JSON endpoints and the discovery documents are\n  unauthenticated; and (2) the Shopify customer-account OpenID Connect provider,\n  whose metadata this origin publishes and whose authorization server is\n  Shopify's, not SAMBAZON's. The UCP/MCP endpoint is a third case: it is not\n  key- or token-gated but PROFILE-gated — it requires the calling agent to\n  present a resolvable UCP agent profile URI before it will do anything.\nschemes:\n  - id: none\n    type: none\n    applies_to:\n      - https://www.sambazon.com/products.json\n\
  \      - https://www.sambazon.com/products/{handle}.json\n      - https://www.sambazon.com/collections/{handle}/products.json\n      - https://www.sambazon.com/search/suggest.json\n      - https://www.sambazon.com/.well-known/ucp\n      - https://www.sambazon.com/llms.txt\n      - https://www.sambazon.com/agents.md\n    description: >-\n      Read-only browsing requires no authentication. The store's own llms.txt\n      documents these under the heading \"Read-Only Browsing (No Authentication\n      Required)\". Verified with anonymous GETs returning 200 application/json.\n  - id: ucp_agent_profile\n    type: agent-identity\n    applies_to:\n      - https://www.sambazon.com/api/ucp/mcp\n    description: >-\n      The UCP/MCP endpoint rejects anonymous JSON-RPC with error -32001\n      \"UCP discovery failed\" / data.code \"invalid_profile_url\" / \"Missing\n      profile uri\". This is an agent-identity gate defined by the Universal\n      Commerce Protocol rather than a conventional API\
  \ credential — the caller\n      must be a registered agent with a fetchable profile. The store publishes\n      no instructions for obtaining one; agents.md simply says to call\n      tools/list.\n    spec: https://ucp.dev/2026-04-08/specification/overview/\n    observed_http_status: 422\n  - id: shopify_customer_account_oidc\n    type: openIdConnect\n    openIdConnectUrl: https://www.sambazon.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/52008485056\n    authorization_endpoint: https://shopify.com/authentication/52008485056/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/52008485056/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/52008485056/logout\n    jwks_uri: https://shopify.com/authentication/52008485056/.well-known/jwks.json\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    response_types_supported: [code]\n\
  \    token_endpoint_auth_methods_supported: [client_secret_basic]\n    code_challenge_methods_supported: [S256]\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n    scopes: ../scopes/sambazon-scopes.yml\n    description: >-\n      Shopify's customer-account identity provider, discoverable from this\n      origin. Governs shopper login on www.sambazon.com/account/login and the\n      customer-account API/MCP scopes. The authorization server and the login\n      UI are Shopify's; SAMBAZON operates neither.\nprotected_resource:\n  spec: RFC 9728\n  document: https://www.sambazon.com/.well-known/oauth-protected-resource\n  resource: https://www.sambazon.com\n  authorization_servers:\n    - https://shopify.com/authentication/52008485056\n  bearer_methods_supported: [header]\nnot_present:\n  - No API key issuance, developer portal, or credential self-service.\n  - No\
  \ mutualTLS, no HTTP basic, no signed-request scheme documented.\n  - No /.well-known/security.txt (404), so no machine-readable security contact.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n    - url: https://www.sambazon.com/.well-known/openid-configuration\n      http_status: 200\n      content_type: application/json; charset=utf-8\n    - url: https://www.sambazon.com/.well-known/oauth-authorization-server\n      http_status: 200\n      content_type: application/json; charset=utf-8\n    - url: https://www.sambazon.com/.well-known/oauth-protected-resource\n      http_status: 200\n      content_type: application/json; charset=utf-8\n    - url: https://www.sambazon.com/api/ucp/mcp\n      http_status: 422\n      content_type: application/json; charset=utf-8\n    - url: https://www.sambazon.com/products.json?limit=1\n      http_status: 200\n      content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sambazon/refs/heads/main/authentication/sambazon-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Ecommerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Retail
- Sustainability
---
