---
anonymous_access: true
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Virtuix Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: Virtuix secures its APIs with none, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: Virtuix
provider_slug: virtuix
scheme_count: 4
schemes:
- applies_to: https://virtuix.com/api/ucp/mcp
  name: anonymous-mcp
  observed: An unauthenticated POST of tools/list and of tools/call search_catalog both returned HTTP 200 with real data on 2026-09-04. Catalog, cart and checkout creation are reachable with no credential; buyer-identity-bound operations are the ones that need the customer token below.
  sources:
  - probe
  type: none
- authorization_endpoint: https://shopify.com/authentication/60989898907/oauth/authorize
  bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/60989898907/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/60989898907
  jwks_uri: https://shopify.com/authentication/60989898907/.well-known/jwks.json
  name: shopify-customer-account-oidc
  note: Storefront customer-account identity for the Virtuix shop, issued by the Shopify platform on behalf of this merchant. Virtuix serves the discovery documents from its own hosts; the authorization server is Shopify's.
  openIdConnectUrl: https://www.virtuix.com/.well-known/openid-configuration
  protected_resource: https://www.virtuix.com
  sources:
  - well-known/virtuix-openid-configuration.json
  - well-known/virtuix-oauth-protected-resource.json
  token_endpoint: https://shopify.com/authentication/60989898907/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- applies_to: Omni One game platform services (Unity/Unreal SDK)
  name: omni-one-oidc-connection
  note: The Omni One Unity SDK changelog records "Added OIDC connection functionality" in 1.1.2 and the docs carry unity-porting-openid / unreal-online-identity pages, but no issuer, authorization endpoint, or discovery document for the Omni One platform is published anywhere public. The identity flow is reached through the licensed SDK and the Omni Dev developer portal only.
  sources:
  - https://docs.virtuix.com/unity-changelog/index.html
  status: documented-not-discoverable
  type: openIdConnect
- applies_to: Omni One Entitlement Check
  name: omni-one-entitlement-key
  note: Each published Omni One title is issued an "Entitlement Key" on the Omni Dev developer portal and verifies purchase at launch through the SDK. The key is issued per game project behind the portal login; no public key format, header name, or endpoint is documented.
  sources:
  - https://docs.virtuix.com/unity-entitlement-check/index.html
  status: gated
  type: apiKey
slug: virtuix-authentication
source_filename: virtuix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://www.virtuix.com/.well-known/openid-configuration,\n  https://www.virtuix.com/.well-known/oauth-protected-resource,\n  https://virtuix.com/api/ucp/mcp (anonymous tools/list),\n  https://docs.virtuix.com/unity-changelog/index.html\ndocs: https://docs.virtuix.com/\nnote: >-\n  No OpenAPI exists for Virtuix, so nothing here is derived from securitySchemes. Every scheme below\n  was read from a discovery document served by a Virtuix host or observed on a live request.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer]\nschemes:\n  - name: anonymous-mcp\n    type: none\n    applies_to: https://virtuix.com/api/ucp/mcp\n    observed: >-\n      An unauthenticated POST of tools/list and of tools/call search_catalog both returned HTTP 200\n      with real data on 2026-09-04. Catalog, cart and checkout creation are reachable with no\n      credential;\
  \ buyer-identity-bound operations are the ones that need the customer token below.\n    sources: [probe]\n  - name: shopify-customer-account-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://www.virtuix.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/60989898907\n    authorization_endpoint: https://shopify.com/authentication/60989898907/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/60989898907/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/60989898907/logout\n    jwks_uri: https://shopify.com/authentication/60989898907/.well-known/jwks.json\n    id_token_signing_alg_values_supported: [RS256]\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    bearer_methods_supported: [header]\n    protected_resource:\
  \ https://www.virtuix.com\n    note: >-\n      Storefront customer-account identity for the Virtuix shop, issued by the Shopify platform on\n      behalf of this merchant. Virtuix serves the discovery documents from its own hosts; the\n      authorization server is Shopify's.\n    sources: [well-known/virtuix-openid-configuration.json, well-known/virtuix-oauth-protected-resource.json]\n  - name: omni-one-oidc-connection\n    type: openIdConnect\n    applies_to: Omni One game platform services (Unity/Unreal SDK)\n    status: documented-not-discoverable\n    note: >-\n      The Omni One Unity SDK changelog records \"Added OIDC connection functionality\" in 1.1.2 and the\n      docs carry unity-porting-openid / unreal-online-identity pages, but no issuer, authorization\n      endpoint, or discovery document for the Omni One platform is published anywhere public. The\n      identity flow is reached through the licensed SDK and the Omni Dev developer portal only.\n    sources: ['https://docs.virtuix.com/unity-changelog/index.html']\n\
  \  - name: omni-one-entitlement-key\n    type: apiKey\n    applies_to: Omni One Entitlement Check\n    status: gated\n    note: >-\n      Each published Omni One title is issued an \"Entitlement Key\" on the Omni Dev developer portal\n      and verifies purchase at launch through the SDK. The key is issued per game project behind the\n      portal login; no public key format, header name, or endpoint is documented.\n    sources: ['https://docs.virtuix.com/unity-entitlement-check/index.html']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtuix/refs/heads/main/authentication/virtuix-authentication.yml
summary_line: none/oauth2/openIdConnect · 4 schemes
tags:
- Virtual Reality
- Gaming
- Hardware
- Agent Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Esports
- Game Development
- Location Based Entertainment
- Consumer Electronics
---
