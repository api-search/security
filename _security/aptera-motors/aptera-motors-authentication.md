---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Aptera Motors Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Aptera Motors secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Aptera Motors
provider_slug: aptera-motors
scheme_count: 3
schemes:
- authorizationUrl: https://shopify.com/authentication/85136474359/oauth/authorize
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
  endSessionUrl: https://shopify.com/authentication/85136474359/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/85136474359
  jwksUri: https://shopify.com/authentication/85136474359/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://shop.aptera.us/.well-known/openid-configuration
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
  - well-known/aptera-motors-shop-openid-configuration.json
  subject_types:
  - public
  tokenUrl: https://shopify.com/authentication/85136474359/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- authorization_servers:
  - https://shopify.com/authentication/85136474359
  bearer_methods_supported:
  - header
  name: shopify-oauth-protected-resource
  resource: https://shop.aptera.us
  sources:
  - well-known/aptera-motors-shop-oauth-protected-resource.json
  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata
  type: oauth2
- authorization_endpoint: https://aptera.us/wp-admin/authorize-application.php
  host: https://aptera.us
  name: wordpress-application-passwords
  note: Advertised by the WordPress REST index at /wp-json/. Gates the wp-abilities/v1 and mcp namespaces, which return HTTP 401 rest_forbidden anonymously. Not a developer-facing authentication method — it is CMS administration.
  scheme: basic
  sources:
  - https://aptera.us/wp-json/
  status: gated
  type: http
slug: aptera-motors-authentication
source_filename: aptera-motors-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: well-known/aptera-motors-shop-openid-configuration.json, well-known/aptera-motors-shop-oauth-authorization-server.json,\n  well-known/aptera-motors-shop-oauth-protected-resource.json\nnote: >-\n  Derived from the OAuth 2.0 / OpenID Connect discovery documents served anonymously\n  from https://shop.aptera.us. Aptera publishes no OpenAPI and no developer\n  authentication documentation; this profile describes the Shopify customer-account\n  authorization server backing the merchandise storefront and its MCP surface. The\n  corporate site (aptera.us) exposes no authenticated API surface beyond a gated\n  WordPress REST/MCP adapter that uses WordPress application passwords.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces:\n  - https://shop.aptera.us/api/mcp (MCP tools/list and catalog tools answer without\n      a token)\n  - https://shop.aptera.us/products.json\
  \ (public Shopify product feed)\n  - https://aptera.us/wp-json/wp/v2 (public WordPress REST read surface)\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://shop.aptera.us/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/85136474359\n  authorizationUrl: https://shopify.com/authentication/85136474359/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/85136474359/oauth/token\n  endSessionUrl: https://shopify.com/authentication/85136474359/logout\n  jwksUri: https://shopify.com/authentication/85136474359/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: [openid, email, 'customer-account-api:full',\
  \ 'customer-account-mcp-api:full']\n  sources: [well-known/aptera-motors-shop-openid-configuration.json]\n- name: shopify-oauth-protected-resource\n  type: oauth2\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  resource: https://shop.aptera.us\n  authorization_servers: [https://shopify.com/authentication/85136474359]\n  bearer_methods_supported: [header]\n  sources: [well-known/aptera-motors-shop-oauth-protected-resource.json]\n- name: wordpress-application-passwords\n  type: http\n  scheme: basic\n  status: gated\n  host: https://aptera.us\n  authorization_endpoint: https://aptera.us/wp-admin/authorize-application.php\n  note: >-\n    Advertised by the WordPress REST index at /wp-json/. Gates the wp-abilities/v1\n    and mcp namespaces, which return HTTP 401 rest_forbidden anonymously. Not a\n    developer-facing authentication method — it is CMS administration.\n  sources: [https://aptera.us/wp-json/]\nx-evidence:\n  fetched: '2026-08-02'\n  discovery_documents_http_status:\
  \ 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptera-motors/refs/heads/main/authentication/aptera-motors-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Automotive
- Electric Vehicles
- Solar
- Manufacturing
- Clean Energy
- Transportation
- Consumer Products
- Mobility
---
