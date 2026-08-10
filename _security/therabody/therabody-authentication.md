---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Therabody Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Therabody secures its APIs with oauth2 and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Therabody
provider_slug: therabody
scheme_count: 4
schemes:
- authorizationUrl: https://account.therabody.com/authentication/oauth/authorize
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
  end_session_endpoint: https://account.therabody.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/67140976867
  jwks_uri: https://account.therabody.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.therabody.com/.well-known/openid-configuration
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
  - well-known/therabody-openid-configuration.json
  tokenUrl: https://account.therabody.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- bearer_methods:
  - header
  description: Bearer token issued by the customer-account authorization server, presented in the Authorization header.
  name: CustomerAccountBearer
  protected_resources:
  - https://www.therabody.com
  - https://account.therabody.com
  scheme: bearer
  sources:
  - well-known/therabody-oauth-protected-resource.json
  type: http
- description: Not a credential. Every UCP MCP tool requires a meta.ucp-agent.profile URI identifying the calling agent, used for agent-profile discovery rather than authentication.
  name: UCPAgentProfile
  sources:
  - mcp/therabody-ucp-mcp-tools.json
  type: other
- description: The Storefront GraphQL endpoint served at /api/<version>/graphql.json answered anonymous introspection and queries without a Storefront access token during probing.
  name: StorefrontAnonymous
  sources:
  - graphql/therabody-storefront.graphql
  type: other
slug: therabody-authentication
source_filename: therabody-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://www.therabody.com/.well-known/openid-configuration\ndocs: https://account.therabody.com/\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  anonymous_surfaces:\n  - Storefront GraphQL introspection\n  - UCP MCP tools/list\n  - Customer Account MCP tools/list\n  - UCP catalog tools\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.therabody.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/67140976867\n  authorizationUrl: https://account.therabody.com/authentication/oauth/authorize\n  tokenUrl: https://account.therabody.com/authentication/oauth/token\n  jwks_uri: https://account.therabody.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.therabody.com/authentication/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  response_types:\n  - code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  pkce:\n  - S256\n  id_token_signing_alg:\n  - RS256\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/therabody-openid-configuration.json\n- name: CustomerAccountBearer\n  type: http\n  scheme: bearer\n  description: Bearer token issued by the customer-account authorization server, presented in the Authorization\n    header.\n  bearer_methods:\n  - header\n  protected_resources:\n  - https://www.therabody.com\n  - https://account.therabody.com\n  sources:\n  - well-known/therabody-oauth-protected-resource.json\n- name: UCPAgentProfile\n  type: other\n  description: Not a credential. Every UCP MCP tool requires a meta.ucp-agent.profile URI identifying\n    the calling agent, used for agent-profile discovery rather than\
  \ authentication.\n  sources:\n  - mcp/therabody-ucp-mcp-tools.json\n- name: StorefrontAnonymous\n  type: other\n  description: The Storefront GraphQL endpoint served at /api/<version>/graphql.json answered anonymous\n    introspection and queries without a Storefront access token during probing.\n  sources:\n  - graphql/therabody-storefront.graphql\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/therabody/refs/heads/main/authentication/therabody-authentication.yml
summary_line: oauth2/openIdConnect · 4 schemes
tags:
- Company
- Wellness
- Health
- Consumer Products
- E-Commerce
- Retail
- Shopify
- Agentic Commerce
- Model Context Protocol
- GraphQL
- Universal Commerce Protocol
---
