---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: probed
name: Swiftly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swiftly secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Swiftly
provider_slug: swiftly
scheme_count: 2
schemes:
- description: 'Per-tenant (retailer chain) key the Swiftly client sends on every GraphQL call. Without a chain context the API returns "IllegalStateException: Chain not available in session context".'
  evidence: Header literal "X-Swiftly-Account-Key" found in https://savemart.com/build/entry.client-UHAB2OGQ.js (Swiftly-built storefront)
  in: header
  name: SwiftlyAccountKey
  parameter_name: X-Swiftly-Account-Key
  sources:
  - graphql/swiftly-shopper.graphql
  type: apiKey
- description: 'Shopper-scoped access token carried in the Authorization header. Required for shopper-account, loyalty-account and reward mutations. Anonymous calls to those fields return "InvalidTokenException: Invalid access token."'
  evidence: POST {getShopperAccount(swiftlyShopperId:"test"){__typename}} to https://prod.swiftlyapi.net/graphql returned InvalidTokenException (HTTP 200, GraphQL errors[])
  name: BearerToken
  scheme: bearer
  sources:
  - graphql/swiftly-shopper.graphql
  type: http
slug: swiftly-authentication
source_filename: swiftly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: >-\n  live probes of https://prod.swiftlyapi.net/graphql plus the first-party Swiftly web\n  client bundle shipped on savemart.com (a Swiftly-built storefront)\ndocs: null\ndocs_note: >-\n  Swiftly publishes no authentication documentation. There is no developer portal, no\n  API reference and no /.well-known/openid-configuration or\n  /.well-known/oauth-authorization-server on any Swiftly host (both 404). Everything\n  below was observed from live responses and from the JavaScript Swiftly ships to\n  shopper browsers — it is not a provider claim.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  anonymous_introspection: true\nschemes:\n- name: SwiftlyAccountKey\n  type: apiKey\n  in: header\n  parameter_name: X-Swiftly-Account-Key\n  description: >-\n    Per-tenant (retailer chain) key the Swiftly client sends on every GraphQL call. Without\n    a chain context the API returns\n    \"IllegalStateException:\
  \ Chain not available in session context\".\n  evidence: >-\n    Header literal \"X-Swiftly-Account-Key\" found in\n    https://savemart.com/build/entry.client-UHAB2OGQ.js (Swiftly-built storefront)\n  sources: [graphql/swiftly-shopper.graphql]\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Shopper-scoped access token carried in the Authorization header. Required for\n    shopper-account, loyalty-account and reward mutations. Anonymous calls to those\n    fields return \"InvalidTokenException: Invalid access token.\"\n  evidence: >-\n    POST {getShopperAccount(swiftlyShopperId:\"test\"){__typename}} to\n    https://prod.swiftlyapi.net/graphql returned InvalidTokenException (HTTP 200,\n    GraphQL errors[])\n  sources: [graphql/swiftly-shopper.graphql]\ncontext_headers:\n- name: X-Swiftly-Account-Key\n  purpose: retailer chain / tenant selection\n- name: X-Swiftly-User-Agent\n  purpose: client identification\n- name: X-Swiftly-Lat\n  purpose: shopper latitude,\
  \ used for store resolution\n- name: X-Swiftly-Lng\n  purpose: shopper longitude, used for store resolution\nopen_surface:\n  introspection: true\n  note: >-\n    GraphQL introspection is enabled for anonymous callers and returns the full 308-type\n    schema (45 queries, 11 mutations). Schema discovery therefore requires no credential;\n    data access does.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://prod.swiftlyapi.net/graphql\n  http_status: 200\n  probes:\n  - {url: 'https://prod.swiftlyapi.net/.well-known/openid-configuration', http_status: 404}\n  - {url: 'https://prod.swiftlyapi.net/.well-known/oauth-authorization-server', http_status: 404}\n  - {url: 'https://swiftly.com/.well-known/openid-configuration', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftly/refs/heads/main/authentication/swiftly-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Retail
- Retail Media
- Grocery
- Advertising
- Loyalty
- Coupons
- Commerce
- Artificial Intelligence
- Mobile
- Company
---
