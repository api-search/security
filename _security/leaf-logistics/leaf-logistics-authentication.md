---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Leaf Logistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leaf Logistics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Leaf Logistics
provider_slug: leaf-logistics
scheme_count: 2
schemes:
- bearer_format: JWT
  evidence: Anonymous POST to /v1/graphql returns HTTP 200 with body {"errors":[{"message":"Missing 'Authorization' or 'Cookie' header in JWT authentication mode", "extensions":{"path":"$","code":"invalid-headers"}}]} — Hasura's HASURA_GRAPHQL_JWT_SECRET mode.
  header: Authorization
  in: header
  name: jwt
  observed: true
  scheme: bearer
  type: http
- evidence: The same error names "Cookie" as an accepted alternative to the Authorization header, which is how the app.leaflogistics.com single-page application authenticates against the same endpoint.
  in: cookie
  name: cookie
  observed: true
  type: apiKey
slug: leaf-logistics-authentication
source_filename: leaf-logistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://api.leaflogistics.com/v1/graphql\nnote: >-\n  DERIVED FROM LIVE PROBES, NOT FROM A PUBLISHED SPEC. Leaf Logistics publishes no developer portal\n  and no authentication documentation, so this profile records only what the API host itself\n  disclosed to an anonymous request. Nothing here is inferred beyond the verbatim error bodies.\napi: Leaf Logistics Platform API\nbase_url: https://api.leaflogistics.com/v1/graphql\nengine:\n  product: Hasura GraphQL Engine\n  version: v2.35.1\n  server_type: ce\n  console_type: pro-lite\n  evidence: >-\n    https://api.leaflogistics.com/v1/version returned {\"server_type\":\"ce\",\"version\":\"v2.35.1\"};\n    https://api.leaflogistics.com/console embeds window.__env with serverVersion \"v2.35.1\" and\n    consoleType \"pro-lite\".\nschemes:\n- name: jwt\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  observed: true\n  evidence: >-\n\
  \    Anonymous POST to /v1/graphql returns HTTP 200 with body\n    {\"errors\":[{\"message\":\"Missing 'Authorization' or 'Cookie' header in JWT authentication mode\",\n    \"extensions\":{\"path\":\"$\",\"code\":\"invalid-headers\"}}]} — Hasura's HASURA_GRAPHQL_JWT_SECRET mode.\n- name: cookie\n  type: apiKey\n  in: cookie\n  observed: true\n  evidence: >-\n    The same error names \"Cookie\" as an accepted alternative to the Authorization header, which is\n    how the app.leaflogistics.com single-page application authenticates against the same endpoint.\noauth2: unknown\nopenid_connect: unknown\nissuer_discovery:\n  checked:\n  - url: https://api.leaflogistics.com/.well-known/openid-configuration\n    status: 404\n  - url: https://www.leaflogistics.com/.well-known/openid-configuration\n    status: 403\n  - url: https://api.leaflogistics.com/.well-known/oauth-authorization-server\n    status: 404\n  result: >-\n    No discovery document is served on any host, so the JWT issuer, signing\
  \ keys and any scope\n    vocabulary could not be established anonymously.\ndocs: null\ndocs_note: >-\n  No public authentication reference exists. Leaf's shipper FAQ says only that it will integrate\n  \"through email, phone, fax, EDI, API — whatever you prefer\"\n  (https://www.leaflogistics.com/shippers/), i.e. credentials and integration detail are handled in\n  onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaf-logistics/refs/heads/main/authentication/leaf-logistics-authentication.yml
summary_line: 2 schemes
tags:
- Logistics
- Freight
- Transportation
- Supply Chain
- Shipping
- Fleet Management
- Sustainability
- GraphQL
---
