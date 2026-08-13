---
api_key_in: []
auth_types: []
description: There is no Evolved By Nature developer program, API key issuance, or auth documentation. The only authentication surface is the Shopify Customer Accounts OAuth 2.0 / OpenID Connect provider behind the two storefronts, advertised from each storefront host via RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata.
kind: authentication
layout: security
method: probed
name: Evolved By Nature Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evolved By Nature declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Evolved By Nature
provider_slug: evolved-by-nature
scheme_count: 2
schemes:
- applies_to:
  - authorization_endpoint: https://shopify.com/authentication/62086119623/oauth/authorize
    end_session_endpoint: https://shopify.com/authentication/62086119623/logout
    issuer: https://shopify.com/authentication/62086119623
    jwks_uri: https://shopify.com/authentication/62086119623/.well-known/jwks.json
    resource: https://skincare.evolvedbynature.com
    token_endpoint: https://shopify.com/authentication/62086119623/oauth/token
  - authorization_endpoint: https://shopify.com/authentication/65777369280/oauth/authorize
    end_session_endpoint: https://shopify.com/authentication/65777369280/logout
    issuer: https://shopify.com/authentication/65777369280
    jwks_uri: https://shopify.com/authentication/65777369280/.well-known/jwks.json
    resource: https://bioactives.evolvedbynature.com
    token_endpoint: https://shopify.com/authentication/65777369280/oauth/token
  bearer_methods_supported:
  - header
  flows:
    authorizationCode:
      code_challenge_methods:
      - S256
      grant_types:
      - authorization_code
      - refresh_token
      - urn:ietf:params:oauth:grant-type:jwt-bearer
      id_token_signing_alg:
      - RS256
      pkce: required
      token_endpoint_auth_methods:
      - client_secret_basic
  id: shopify-customer-accounts-oauth2
  standard: OAuth 2.0 + OpenID Connect
  type: oauth2
- id: anonymous-discovery
  note: MCP `tools/list` and `initialize`, GraphQL introspection, /.well-known/*, /llms.txt, /agents.md and /products.json all answer with no credentials. Discovery is open; transacting on a buyer's behalf is not.
  type: none
slug: evolved-by-nature-authentication
source_filename: evolved-by-nature-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://skincare.evolvedbynature.com/.well-known/oauth-authorization-server and\n  /.well-known/oauth-protected-resource (HTTP 200, unauthenticated, 2026-08-12)\nname: Evolved By Nature — authentication profile\ndescription: >-\n  There is no Evolved By Nature developer program, API key issuance, or auth documentation. The only\n  authentication surface is the Shopify Customer Accounts OAuth 2.0 / OpenID Connect provider behind\n  the two storefronts, advertised from each storefront host via RFC 8414 authorization-server\n  metadata and RFC 9728 protected-resource metadata.\nownership_note: >-\n  Authorization servers are hosted by Shopify (shopify.com/authentication/<shop-id>) and are named by\n  metadata documents served from Evolved By Nature's own hosts. The shop ids are Evolved By Nature's.\nschemes:\n- id: shopify-customer-accounts-oauth2\n  type: oauth2\n  standard: OAuth 2.0 + OpenID Connect\n  flows:\n    authorizationCode:\n\
  \      pkce: required\n      code_challenge_methods: [S256]\n      grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n      token_endpoint_auth_methods: [client_secret_basic]\n      id_token_signing_alg: [RS256]\n  applies_to:\n  - resource: https://skincare.evolvedbynature.com\n    issuer: https://shopify.com/authentication/62086119623\n    authorization_endpoint: https://shopify.com/authentication/62086119623/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/62086119623/oauth/token\n    jwks_uri: https://shopify.com/authentication/62086119623/.well-known/jwks.json\n    end_session_endpoint: https://shopify.com/authentication/62086119623/logout\n  - resource: https://bioactives.evolvedbynature.com\n    issuer: https://shopify.com/authentication/65777369280\n    authorization_endpoint: https://shopify.com/authentication/65777369280/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/65777369280/oauth/token\n\
  \    jwks_uri: https://shopify.com/authentication/65777369280/.well-known/jwks.json\n    end_session_endpoint: https://shopify.com/authentication/65777369280/logout\n  bearer_methods_supported: [header]\n- id: anonymous-discovery\n  type: none\n  note: >-\n    MCP `tools/list` and `initialize`, GraphQL introspection, /.well-known/*, /llms.txt, /agents.md\n    and /products.json all answer with no credentials. Discovery is open; transacting on a buyer's\n    behalf is not.\nunauthenticated_surfaces:\n- https://skincare.evolvedbynature.com/api/ucp/mcp\n- https://skincare.evolvedbynature.com/api/mcp\n- https://bioactives.evolvedbynature.com/api/ucp/mcp\n- https://bioactives.evolvedbynature.com/api/mcp\n- https://skincare.evolvedbynature.com/api/2025-07/graphql.json\n- https://bioactives.evolvedbynature.com/api/2025-07/graphql.json\ngaps:\n- No provider-published authentication documentation of any kind.\n- No API key programme, no partner credentials, no developer portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolved-by-nature/refs/heads/main/authentication/evolved-by-nature-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Materials Science
- Sustainability
- Personal Care
- Cosmetics
- Specialty Chemicals
- Textiles
- eCommerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
---
