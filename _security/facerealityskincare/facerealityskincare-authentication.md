---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: Authentication profile for the Shopify Customer Account API fronting Face Reality Skincare's store. Captured from the live OIDC/OAuth 2.0 discovery documents. The unauthenticated Storefront MCP shop tools (mcp/) require no auth; customer-account and MCP write scopes are obtained via the OAuth 2.0 Authorization Code flow with PKCE below.
kind: authentication
layout: security
method: searched
name: Facerealityskincare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Face Reality Skincare secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Face Reality Skincare
provider_slug: facerealityskincare
scheme_count: 2
schemes:
- authorizationUrl: https://account.facerealityskincare.com/authentication/oauth/authorize
  end_session_endpoint: https://account.facerealityskincare.com/authentication/logout
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/7860748377
  name: shopifyCustomerAccountOAuth
  pkce: S256
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: well-known/facerealityskincare-oauth-authorization-server.json
  tokenUrl: https://account.facerealityskincare.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
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
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/7860748377
  jwks_uri: https://account.facerealityskincare.com/authentication/.well-known/jwks.json
  name: shopifyOpenIDConnect
  openIdConnectUrl: https://facerealityskincare.com/.well-known/openid-configuration
  source: well-known/facerealityskincare-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
slug: facerealityskincare-authentication
source_filename: facerealityskincare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://facerealityskincare.com/.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server (Shopify Customer Account API discovery)\ndescription: >-\n  Authentication profile for the Shopify Customer Account API fronting Face\n  Reality Skincare's store. Captured from the live OIDC/OAuth 2.0 discovery\n  documents. The unauthenticated Storefront MCP shop tools (mcp/) require no\n  auth; customer-account and MCP write scopes are obtained via the OAuth 2.0\n  Authorization Code flow with PKCE below.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\nschemes:\n- name: shopifyCustomerAccountOAuth\n  type: oauth2\n  flow: authorizationCode\n  issuer: https://shopify.com/authentication/7860748377\n  authorizationUrl: https://account.facerealityskincare.com/authentication/oauth/authorize\n  tokenUrl: https://account.facerealityskincare.com/authentication/oauth/token\n  end_session_endpoint: https://account.facerealityskincare.com/authentication/logout\n\
  \  pkce: S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  source: well-known/facerealityskincare-oauth-authorization-server.json\n- name: shopifyOpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://facerealityskincare.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/7860748377\n  jwks_uri: https://account.facerealityskincare.com/authentication/.well-known/jwks.json\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  source: well-known/facerealityskincare-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facerealityskincare/refs/heads/main/authentication/facerealityskincare-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Skincare
- Beauty
- Cosmetics
- Ecommerce
- Shopify
- Commerce
- Agent Commerce
- MCP
---
