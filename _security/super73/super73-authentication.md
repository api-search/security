---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Super73 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Super73 declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Super73
provider_slug: super73
scheme_count: 3
schemes:
- applies_to:
  - https://super73.com/api/ucp/mcp (tools/list, catalog, cart)
  - https://super73.com/api/2025-07/graphql.json (introspection and read queries)
  - https://super73.com/products.json and the other read-only storefront JSON endpoints
  id: anonymous
  note: Confirmed by successful unauthenticated calls on 2026-08-29.
  type: none
  verified: probed
- applies_to:
  - buyer identity, saved addresses and payment methods
  - order retrieval (get_order)
  authorization_endpoint: https://shopify.com/authentication/13743231/oauth/authorize
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oidc
  id_token_signing_algs:
  - RS256
  issuer: https://shopify.com/authentication/13743231
  jwks_uri: https://shopify.com/authentication/13743231/.well-known/jwks.json
  note: The protected resource https://super73.com declares bearer_methods_supported ["header"] and names this issuer as its authorization server, so RFC 9728 protected-resource metadata is served correctly.
  openid_configuration: https://super73.com/.well-known/openid-configuration
  pkce: S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types:
  - public
  token_endpoint: https://shopify.com/authentication/13743231/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- applies_to:
  - payment
  id: shop-pay-delegated
  note: The store's own agent instructions direct personal shopping agents to route payment through the Shop skill (https://shop.app/SKILL.md) and Shop Pay so the agent never handles card data, and state that agents must not complete payment without explicit buyer consent.
  source: https://super73.com/agents.md
  type: delegated
  verified: searched
slug: super73-authentication
source_filename: super73-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  https://super73.com/.well-known/openid-configuration, /.well-known/oauth-authorization-server and\n  /.well-known/oauth-protected-resource (all HTTP 200, 2026-08-29), plus live anonymous calls to\n  /api/ucp/mcp and /api/2025-07/graphql.json\nsummary: >-\n  SUPER73's agent surfaces are tiered. Catalog and cart operations on the MCP endpoint, and read queries\n  plus introspection on the Storefront GraphQL endpoint, require NO credential at all. Buyer-scoped\n  operations (customer account, saved addresses, order retrieval) escalate to a full OpenID Connect\n  authorization-code + PKCE flow hosted by Shopify on behalf of the merchant. Payment completion is\n  additionally gated on contemporaneous human approval, which is a policy control rather than a\n  credential.\nschemes:\n- id: anonymous\n  type: none\n  applies_to:\n  - https://super73.com/api/ucp/mcp (tools/list, catalog, cart)\n  - https://super73.com/api/2025-07/graphql.json\
  \ (introspection and read queries)\n  - https://super73.com/products.json and the other read-only storefront JSON endpoints\n  verified: probed\n  note: Confirmed by successful unauthenticated calls on 2026-08-29.\n- id: shopify-customer-account-oidc\n  type: openIdConnect\n  flow: authorization_code\n  pkce: S256\n  issuer: https://shopify.com/authentication/13743231\n  openid_configuration: https://super73.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/13743231/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/13743231/oauth/token\n  jwks_uri: https://shopify.com/authentication/13743231/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_algs: [RS256]\n  subject_types: [public]\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n\
  \  - customer-account-mcp-api:full\n  applies_to:\n  - buyer identity, saved addresses and payment methods\n  - order retrieval (get_order)\n  note: >-\n    The protected resource https://super73.com declares bearer_methods_supported [\"header\"] and names this\n    issuer as its authorization server, so RFC 9728 protected-resource metadata is served correctly.\n- id: shop-pay-delegated\n  type: delegated\n  applies_to: [payment]\n  note: >-\n    The store's own agent instructions direct personal shopping agents to route payment through the Shop\n    skill (https://shop.app/SKILL.md) and Shop Pay so the agent never handles card data, and state that\n    agents must not complete payment without explicit buyer consent.\n  verified: searched\n  source: https://super73.com/agents.md\neu_variant:\n  note: >-\n    eu.super73.com serves its own OIDC metadata for SUPER73 BV with a separate Shopify issuer; the model\n    is identical.\n  openid_configuration: https://eu.super73.com/.well-known/openid-configuration\n\
  \  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super73/refs/heads/main/authentication/super73-authentication.yml
summary_line: 3 schemes
tags:
- Electric Bikes
- Micromobility
- E-Commerce
- Agentic Commerce
- Consumer Hardware
- MCP
- Universal Commerce Protocol
- Shopify
- Direct to Consumer
- Internet of Things
- Transportation
---
