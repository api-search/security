---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Paperless Post Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Paperless Post secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Paperless Post
provider_slug: paperless-post
scheme_count: 2
schemes:
- authorization_endpoint: https://shopify.com/authentication/53345157285/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/53345157285/logout
  grant_types_supported:
  - authorization_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/53345157285
  jwks_uri: https://shopify.com/authentication/53345157285/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://partyshop.paperlesspost.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/paperless-post-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/53345157285/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- flows:
  - authorizationUrl: https://shopify.com/authentication/53345157285/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/53345157285/oauth/token
  metadata_url: https://partyshop.paperlesspost.com/.well-known/oauth-authorization-server
  name: shopify-oauth2-authorization-server
  rfc: RFC 8414
  sources:
  - well-known/paperless-post-oauth-authorization-server.json
  type: oauth2
slug: paperless-post-authentication
source_filename: paperless-post-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://partyshop.paperlesspost.com/.well-known/openid-configuration\ndocs: https://partyshop.paperlesspost.com/agents.md\nnote: >-\n  Paperless Post publishes no developer authentication documentation. This\n  profile was probed from the OAuth/OIDC discovery documents served on the\n  Paperless Post Party Shop storefront host (partyshop.paperlesspost.com),\n  which delegates to Shopify's customer-account authorization server. The core\n  invitation product at www.paperlesspost.com has no public authenticated API;\n  its /api/v1 endpoints are session-cookie surfaces for its own first-party web\n  and mobile clients.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  bearer_methods: [header]\n  anonymous_read: true\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://partyshop.paperlesspost.com/.well-known/openid-configuration\n\
  \  issuer: https://shopify.com/authentication/53345157285\n  authorization_endpoint: https://shopify.com/authentication/53345157285/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/53345157285/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/53345157285/logout\n  jwks_uri: https://shopify.com/authentication/53345157285/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [S256]\n  sources: [well-known/paperless-post-openid-configuration.json]\n- name: shopify-oauth2-authorization-server\n  type: oauth2\n  rfc: RFC 8414\n  metadata_url: https://partyshop.paperlesspost.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/53345157285/oauth/authorize\n    tokenUrl:\
  \ https://shopify.com/authentication/53345157285/oauth/token\n  sources: [well-known/paperless-post-oauth-authorization-server.json]\nprotected_resource:\n  rfc: RFC 9728\n  metadata_url: https://partyshop.paperlesspost.com/.well-known/oauth-protected-resource\n  resource: https://partyshop.paperlesspost.com\n  authorization_servers: [https://shopify.com/authentication/53345157285]\n  bearer_methods_supported: [header]\n  sources: [well-known/paperless-post-oauth-protected-resource.json]\nunauthenticated_surface:\n  description: >-\n    The storefront's read-only product/collection JSON endpoints are documented\n    as requiring no authentication.\n  endpoints:\n  - GET https://partyshop.paperlesspost.com/collections/all/products.json\n  - GET https://partyshop.paperlesspost.com/collections/{handle}/products.json\n  - GET https://partyshop.paperlesspost.com/products/{handle}.json\n  - GET https://partyshop.paperlesspost.com/search?q={query}&type=product\n  verified:\n  - {url: 'https://partyshop.paperlesspost.com/collections/all/products.json?limit=2',\n\
  \    http_status: 200, content_type: application/json}\n  source: https://partyshop.paperlesspost.com/agents.md\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - {url: 'https://partyshop.paperlesspost.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://partyshop.paperlesspost.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://partyshop.paperlesspost.com/.well-known/oauth-protected-resource', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperless-post/refs/heads/main/authentication/paperless-post-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Invitations
- Events
- Greeting Cards
- Stationery
- Consumer
- E-Commerce
- RSVP
- Design
---
