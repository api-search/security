---
api_key_in: []
api_specs:
- filename: carmd-openapi.yml
  format: yaml
  label: CarMD Vehicle API
  slug: carmd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carmd/refs/heads/main/openapi/carmd-openapi.yml
auth_types: []
description: 'Authentication profile for every CarMD surface that could actually be reached. There is no OpenAPI to derive securitySchemes from, so every entry below was established by calling the surface. The CarMD Vehicle API''s own auth model could not be verified: its host refused connections.'
kind: authentication
layout: security
method: probed
name: Carmd Authentication
name_suffix: Authentication
oauth_flows: []
overview: CarMD declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CarMD
provider_slug: carmd
scheme_count: 0
schemes: []
slug: carmd-authentication
source_filename: carmd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  live probes 2026-08-27 — https://carmd.com/.well-known/openid-configuration,\n  https://carmd.com/api/ucp/mcp, https://carmd.com/api/2026-04/graphql.json,\n  https://carmd.com/llms.txt; plus https://api.carmd.com/member/docs (unreachable)\nprovider: CarMD\nproviderId: carmd\ndescription: >-\n  Authentication profile for every CarMD surface that could actually be reached. There is no OpenAPI to\n  derive securitySchemes from, so every entry below was established by calling the surface. The CarMD\n  Vehicle API's own auth model could not be verified: its host refused connections.\nsurfaces:\n  - name: CarMD UCP Commerce MCP\n    endpoint: https://carmd.com/api/ucp/mcp\n    scheme_type: none\n    scheme: anonymous\n    verified: probed\n    evidence: >-\n      POST tools/list and POST initialize both returned HTTP 200 with no Authorization header and no API\n      key. No 401/403 challenge was issued.\n    required_context:\n\
  \      - field: meta.ucp-agent.profile\n        in: body\n        required: true\n        description: >-\n          Every tool call must carry a UCP agent profile URI. Omitting it returns HTTP 422 with JSON-RPC\n          error -32001 \"UCP discovery failed\" (data.code invalid_profile_url). This is agent identity\n          discovery, not a credential.\n    payment_authorization: >-\n      Payment on complete_checkout requires contemporaneous human buyer approval; the provider's llms.txt\n      states agents must not complete payment without explicit buyer consent.\n  - name: CarMD Storefront GraphQL\n    endpoint: https://carmd.com/api/2026-04/graphql.json\n    scheme_type: none\n    scheme: anonymous\n    verified: probed\n    evidence: >-\n      Anonymous POST introspection returned the full 424-type schema, and an anonymous data query returned\n      shop.name \"CarMD\" and live product records — both HTTP 200 with no storefront access token supplied.\n    note: >-\n      Customer-scoped\
  \ fields (customer, order history) still require a customer access token minted through\n      customerAccessTokenCreate or the OIDC flow below.\n  - name: CarMD customer accounts (OpenID Connect)\n    endpoint: https://shopify.com/authentication/93440671876\n    discovery: https://carmd.com/.well-known/openid-configuration\n    scheme_type: openIdConnect\n    scheme: 'OAuth 2.0 authorization code + PKCE (S256)'\n    verified: probed\n    flows:\n      authorization_code:\n        authorization_url: https://shopify.com/authentication/93440671876/oauth/authorize\n        token_url: https://shopify.com/authentication/93440671876/oauth/token\n        refresh_url: https://shopify.com/authentication/93440671876/oauth/token\n        scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    client_auth: [client_secret_basic, client_secret_post]\n    token_format: 'JWT (RS256 id_token)'\n    scopes_artifact: scopes/carmd-scopes.yml\n  - name: CarMD Vehicle API\
  \ (CarScan)\n    endpoint: https://api.carmd.com/\n    human_url: https://api.carmd.com/member/\n    scheme_type: unknown\n    scheme: unverified\n    verified: none\n    evidence: >-\n      Host DNS-resolves to 54.86.119.234 but TCP 80 and 443 are closed. curl returned \"Connection timed\n      out after 8001 milliseconds\" and an independent fetcher returned ECONNREFUSED on 54.86.119.234:443.\n      The developer documentation at https://api.carmd.com/member/docs, still linked from the carmd.com\n      footer, could not be retrieved; archive.org was also unreachable from this run.\n    note: >-\n      Search-engine indexed text of that documentation page describes registration issuing two credentials,\n      with an authorization key that must be sent in a request header rather than as a query parameter.\n      That is second-hand and unverified, so it is recorded here as a lead, not as a documented scheme.\nfindings:\n  api_key: unverified\n  oauth2: true\n  openid_connect: true\n \
  \ mutual_tls: false\n  anonymous_surfaces: 2\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carmd/refs/heads/main/authentication/carmd-authentication.yml
summary_line: 0 schemes
tags:
- Automobiles
- Cars
- Diagnostics
- Vehicles
- Automotive
- OBD-II
- Agentic Commerce
- MCP
- E-Commerce
---
