---
api_key_in: []
auth_types:
- bearer-token
description: ''
kind: authentication
layout: security
method: probed
name: Masterworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Masterworks secures its APIs with bearer-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Masterworks
provider_slug: masterworks
scheme_count: 2
schemes:
- args:
  - name: clients
    note: Restricts which first-party client applications may satisfy the guard.
  - name: allowUserToken
    note: Whether an end-user token (as opposed to a service token) satisfies the guard.
  kind: graphql-directive
  locations:
  - FIELD_DEFINITION
  name: authenticate
  sources:
  - graphql/masterworks-schema.graphql
- kind: graphql-directive
  locations:
  - FIELD_DEFINITION
  name: signoutAuth
  note: 'Guards the pre-account onboarding funnel. The signed-out surface is not anonymous either — the `signedOutDashboard` query requires a `userToken: String!` argument, i.e. a funnel token handed to the client earlier in the flow.'
  sources:
  - graphql/masterworks-schema.graphql
slug: masterworks-authentication
source_filename: masterworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://api.masterworks.com/graphql\nnote: >-\n  Derived from the introspected GraphQL schema (graphql/masterworks-schema.graphql) plus live\n  anonymous probes. Masterworks publishes no authentication documentation — there is no developer\n  portal, no API reference and no auth guide — so nothing here comes from provider docs.\n\nsummary:\n  types: [bearer-token]\n  documented_by_provider: false\n  public_developer_credentials: false\n  self_serve_api_keys: false\n  oauth2: false\n  openid_connect: false\n  api_key: false\n  mutual_tls: false\n  scopes: none-published\n\nmodel: >-\n  Authentication is enforced per field by the server-defined @authenticate directive rather than by a\n  declared security scheme (GraphQL has no securitySchemes equivalent). Credentials are user session\n  tokens issued to Masterworks' own first-party clients; the directive takes a `clients` argument,\n  indicating the server also constrains which\
  \ client application a token was minted for. There is no\n  route for a third-party developer to obtain a token: account creation yields an investor session,\n  not an API credential.\n\nschemes:\n- name: authenticate\n  kind: graphql-directive\n  locations: [FIELD_DEFINITION]\n  args:\n  - name: clients\n    note: Restricts which first-party client applications may satisfy the guard.\n  - name: allowUserToken\n    note: Whether an end-user token (as opposed to a service token) satisfies the guard.\n  sources: [graphql/masterworks-schema.graphql]\n- name: signoutAuth\n  kind: graphql-directive\n  locations: [FIELD_DEFINITION]\n  note: >-\n    Guards the pre-account onboarding funnel. The signed-out surface is not anonymous either — the\n    `signedOutDashboard` query requires a `userToken: String!` argument, i.e. a funnel token handed\n    to the client earlier in the flow.\n  sources: [graphql/masterworks-schema.graphql]\n\nobserved_failure:\n  http_status: 200\n  graphql_errors:\n  -\
  \ message: Invalid authentication\n    path: [artists]\n    extensions:\n      reason: invalidToken\n      code: invalidAuthentication\n      status: 401\n  note: >-\n    Errors are returned inside a 200 response body per the GraphQL spec; the transport-level status\n    the API intends is carried in extensions.status.\n\nunauthenticated_surface:\n  introspection: true\n  fields:\n  - health          # returns \"OK\" with no credentials\n  - testQuery\n  note: >-\n    Schema introspection and the `health` liveness field answer anonymously. Every other field\n    probed returned invalidAuthentication.\n\nwell_known:\n  openid_configuration: 404 on api.masterworks.com\n  oauth_authorization_server: 404 on api.masterworks.com\n  note: >-\n    www.masterworks.com answers 200 with an identical 8,531-byte single-page-app shell for every\n    /.well-known/* path, so those 200s are catch-all false positives, not discovery documents.\n\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - url:\
  \ https://api.masterworks.com/graphql\n    http_status: 200\n    note: anonymous introspection succeeded\n  - url: https://api.masterworks.com/graphql\n    http_status: 200\n    note: 'anonymous data query -> code invalidAuthentication (status 401)'\n  - url: https://api.masterworks.com/.well-known/openid-configuration\n    http_status: 404\n  - url: https://api.masterworks.com/.well-known/oauth-authorization-server\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/masterworks/refs/heads/main/authentication/masterworks-authentication.yml
summary_line: bearer-token · 2 schemes
tags:
- Art
- Art Investing
- Alternative Investments
- Fintech
- Investing
- Securities
- Fractional Ownership
- Secondary Market
- Wealth Management
- Regulation A
- GraphQL
---
