---
api_key_in:
- header
auth_types:
- none
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dolls Kill Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Dolls Kill secures its APIs with none, oauth2, openIdConnect, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Dolls Kill
provider_slug: dolls-kill
scheme_count: 4
schemes:
- applies_to:
  - https://www.dollskill.com/api/ucp/mcp (initialize, tools/list)
  - https://www.dollskill.com/api/{version}/graphql.json (introspection and public storefront reads)
  - https://www.dollskill.com/products.json and the /collections/*/products.json family
  - https://www.dollskill.com/.well-known/* discovery documents
  name: Anonymous
  note: No credential of any kind is required to enumerate the MCP tool set with its full input schemas, to introspect the Storefront GraphQL schema, or to read product JSON. This is the widest anonymous machine-readable surface on the property.
  type: none
- applies_to:
  - https://www.dollskill.com/api/ucp/mcp (tools/call, prompts/list, resources/list)
  format: uri
  in: body
  name: UCP agent profile
  note: Not a bearer credential — an HTTP-resolvable agent profile URI the merchant fetches to identify the calling agent. Omitting it returns JSON-RPC -32001 with data.code invalid_profile_url; supplying an unreachable URI returns data.code profile_unreachable. Observed on live probes 2026-08-12.
  parameter: meta.ucp-agent.profile
  type: apiKey
- applies_to:
  - https://www.dollskill.com/api/{version}/graphql.json
  in: header
  name: Shopify Storefront access token
  note: The Storefront API conventionally takes this header, but the Dolls Kill endpoint answered a full introspection query with no token present. Recorded as optional because that is what was observed, not because the docs say so.
  parameter: X-Shopify-Storefront-Access-Token
  required: false
  type: apiKey
- applies_to:
  - https://account.dollskill.com
  - Customer Account API and Customer Account MCP API (order history, addresses)
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
  end_session_endpoint: https://account.dollskill.com/authentication/logout
  flows:
  - authorizationUrl: https://account.dollskill.com/authentication/oauth/authorize
    flow: authorizationCode
    scopes:
      customer-account-api:full: Full access to the Customer Account API
      customer-account-mcp-api:full: Full access to the Customer Account MCP API
      email: Access to the customer's email address
      openid: OpenID Connect authentication
    tokenUrl: https://account.dollskill.com/authentication/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/63463358721
  jwks_uri: https://account.dollskill.com/authentication/.well-known/jwks.json
  name: Customer Account OAuth 2.0 / OpenID Connect
  openid_connect_url: https://www.dollskill.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
slug: dolls-kill-authentication
source_filename: dolls-kill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://www.dollskill.com/.well-known/openid-configuration\ndocs: https://www.dollskill.com/agents.md\nnote: 'Dolls Kill publishes no OpenAPI, so this profile was not derived from securitySchemes.\n  It was read from the live OpenID Connect / OAuth discovery documents the storefront\n  serves, from the RFC 9728 protected-resource metadata, and from probing each API\n  surface anonymously to observe what it actually requires.'\nsummary:\n  types: [none, oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces: 4\n  gated_surfaces: 2\nschemes:\n- name: Anonymous\n  type: none\n  applies_to:\n  - https://www.dollskill.com/api/ucp/mcp (initialize, tools/list)\n  - https://www.dollskill.com/api/{version}/graphql.json (introspection and public\n    storefront reads)\n  - https://www.dollskill.com/products.json and the /collections/*/products.json family\n  - https://www.dollskill.com/.well-known/*\
  \ discovery documents\n  note: 'No credential of any kind is required to enumerate the MCP tool set with its\n    full input schemas, to introspect the Storefront GraphQL schema, or to read product\n    JSON. This is the widest anonymous machine-readable surface on the property.'\n- name: UCP agent profile\n  type: apiKey\n  in: body\n  parameter: meta.ucp-agent.profile\n  format: uri\n  applies_to:\n  - https://www.dollskill.com/api/ucp/mcp (tools/call, prompts/list, resources/list)\n  note: 'Not a bearer credential — an HTTP-resolvable agent profile URI the merchant\n    fetches to identify the calling agent. Omitting it returns JSON-RPC -32001 with\n    data.code invalid_profile_url; supplying an unreachable URI returns data.code\n    profile_unreachable. Observed on live probes 2026-08-12.'\n- name: Shopify Storefront access token\n  type: apiKey\n  in: header\n  parameter: X-Shopify-Storefront-Access-Token\n  applies_to:\n  - https://www.dollskill.com/api/{version}/graphql.json\n\
  \  required: false\n  note: 'The Storefront API conventionally takes this header, but the Dolls Kill endpoint\n    answered a full introspection query with no token present. Recorded as optional\n    because that is what was observed, not because the docs say so.'\n- name: Customer Account OAuth 2.0 / OpenID Connect\n  type: oauth2\n  openid_connect_url: https://www.dollskill.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/63463358721\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.dollskill.com/authentication/oauth/authorize\n    tokenUrl: https://account.dollskill.com/authentication/oauth/token\n    scopes:\n      openid: OpenID Connect authentication\n      email: Access to the customer's email address\n      customer-account-api:full: Full access to the Customer Account API\n      customer-account-mcp-api:full: Full access to the Customer Account MCP API\n  pkce:\n    supported: true\n    code_challenge_methods: [S256]\n\
  \  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  jwks_uri: https://account.dollskill.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.dollskill.com/authentication/logout\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  applies_to:\n  - https://account.dollskill.com\n  - Customer Account API and Customer Account MCP API (order history, addresses)\nprotected_resource:\n  source: https://www.dollskill.com/.well-known/oauth-protected-resource\n  resource: https://www.dollskill.com\n  authorization_servers:\n  - https://account.dollskill.com\n  - https://shopify.com/authentication/63463358721\n  bearer_methods_supported: [header]\nhuman_in_the_loop:\n  required_for: [complete_checkout]\n  statement: 'Checkouts are for humans. Do NOT complete checkout, payment, or order\n    placement automatically\
  \ — no scripted form fills, browser automation, or end-to-end\n    agent flows that finalize payment without an explicit, contemporaneous human approval\n    step.'\n  published_at:\n  - https://www.dollskill.com/robots.txt\n  - https://www.dollskill.com/agents.md\n  - https://www.dollskill.com/llms.txt\nx-evidence:\n- url: https://www.dollskill.com/.well-known/openid-configuration\n  status: 200\n- url: https://www.dollskill.com/.well-known/oauth-protected-resource\n  status: 200\n- url: https://www.dollskill.com/api/ucp/mcp\n  status: 200\n  note: tools/list answered anonymously\n- url: https://www.dollskill.com/api/2026-04/graphql.json\n  status: 200\n  note: full introspection answered with no access token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolls-kill/refs/heads/main/authentication/dolls-kill-authentication.yml
summary_line: none/oauth2/openIdConnect/apiKey · 4 schemes
tags:
- Company
- Retail
- E-Commerce
- Fashion
- Apparel
- Commerce
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- Direct to Consumer
---
