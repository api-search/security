---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- none
description: ''
kind: authentication
layout: security
method: searched
name: Everytable Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Everytable secures its APIs with openIdConnect, oauth2, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Everytable
provider_slug: everytable
scheme_count: 3
schemes:
- authorization_endpoint: https://account.everytable.com/authentication/oauth/authorize
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
  end_session_endpoint: https://account.everytable.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/69951324217
  jwks_uri: https://account.everytable.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://everytable.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/everytable-openid-configuration.json
  - well-known/everytable-oauth-authorization-server.json
  subject_types_supported:
  - public
  token_endpoint: https://account.everytable.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- description: RFC 9728 protected resource metadata at /.well-known/oauth-protected-resource declares bearer_methods_supported = [header] for the resource https://everytable.com.
  name: BearerToken
  scheme: bearer
  sources:
  - well-known/everytable-oauth-protected-resource.json
  type: http
- description: 'The read-only storefront catalog paths Everytable documents in its own llms.txt require no authentication: /products/{handle}.json, /collections/{handle}/products.json, /search?q={query}&type=product, /sitemap.xml.'
  name: Anonymous
  sources:
  - llms/everytable-llms.txt
  type: none
slug: everytable-authentication
source_filename: everytable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://everytable.com/.well-known/openid-configuration\ndocs: https://everytable.com/.well-known/oauth-authorization-server\nnote: Everytable publishes no OpenAPI, so this profile is read from the live, anonymous\n  OAuth/OIDC discovery documents its storefront serves rather than derived from securitySchemes.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - none\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://everytable.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/69951324217\n  authorization_endpoint: https://account.everytable.com/authentication/oauth/authorize\n  token_endpoint: https://account.everytable.com/authentication/oauth/token\n  end_session_endpoint: https://account.everytable.com/authentication/logout\n  jwks_uri: https://account.everytable.com/authentication/.well-known/jwks.json\n\
  \  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/everytable-openid-configuration.json\n  - well-known/everytable-oauth-authorization-server.json\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: RFC 9728 protected resource metadata at /.well-known/oauth-protected-resource\n    declares bearer_methods_supported = [header] for the resource https://everytable.com.\n  sources:\n  - well-known/everytable-oauth-protected-resource.json\n\
  - name: Anonymous\n  type: none\n  description: 'The read-only storefront catalog paths Everytable documents in its\n    own llms.txt require no authentication: /products/{handle}.json, /collections/{handle}/products.json,\n    /search?q={query}&type=product, /sitemap.xml.'\n  sources:\n  - llms/everytable-llms.txt\nprotected_resource:\n  resource: https://everytable.com\n  authorization_servers:\n  - https://account.everytable.com\n  - https://shopify.com/authentication/69951324217\n  bearer_methods_supported:\n  - header\nagent_endpoint_auth:\n  endpoint: https://everytable.com/api/ucp/mcp\n  observed: 'Anonymous POST tools/list returns HTTP 422 with JSON-RPC error -32001\n    (invalid_profile_url) rather than an OAuth challenge — the gate is a required UCP\n    agent profile URI, not a bearer token. Authenticated buyer-scoped operations map\n    to the customer-account-mcp-api:full scope above.'\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://everytable.com/.well-known/openid-configuration\n\
  \    http_status: 200\n  - url: https://everytable.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://everytable.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://account.everytable.com/authentication/.well-known/jwks.json\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everytable/refs/heads/main/authentication/everytable-authentication.yml
summary_line: openIdConnect/oauth2/none · 3 schemes
tags:
- Company
- Food
- Restaurants
- Meal Delivery
- Ecommerce
- Agentic Commerce
- Shopify
- Social Enterprise
- Nutrition
- Subscriptions
---
