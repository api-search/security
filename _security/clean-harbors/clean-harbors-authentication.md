---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Clean Harbors Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clean Harbors declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Clean Harbors
provider_slug: clean-harbors
scheme_count: 5
schemes:
- description: 'No credential of any kind. Every one of the four tools was called anonymously on 2026-09-05 and returned HTTP 200. CORS is wide open (access-control-allow-origin: *), so a browser-resident agent can call it directly.'
  endpoint: https://careers.cleanharbors.com/api/mcp/jobs
  id: careers-anonymous
  surface: Careers Job Query API
  type: none
  verified: probed
- description: The catalog, CMS, store-configuration and guest-cart portion of the schema answers with no credential. Full schema introspection is also anonymous and enabled — the entire 861-type contract was read without a token.
  endpoint: https://store.safety-kleen.com/graphql
  id: commerce-graphql-anonymous
  surface: Clean Harbors / Safety-Kleen commerce GraphQL
  type: none
  verified: probed
- description: Customer-scoped fields (customer, customerCart, customerOrders, company, negotiableQuotes, requisition lists, purchase orders, wishlists) require a customer token. The schema issues one via the generateCustomerToken mutation and revokes it via revokeCustomerToken; generateCustomerTokenAsAdmin exists for delegated impersonation. There is no client-credentials, no OAuth authorization-code flow, and no dynamic client registration in the contract.
  endpoint: https://store.safety-kleen.com/graphql
  format: Bearer <customer token>
  header: Authorization
  id: commerce-graphql-customer-token
  scheme: bearer
  surface: Clean Harbors / Safety-Kleen commerce GraphQL
  token_mutations:
    issue: generateCustomerToken
    issue_delegated: generateCustomerTokenAsAdmin
    revoke: revokeCustomerToken
  type: http
  verified: derived
- description: Almost the whole REST surface is Bearer-gated. GET /rest/V1/store/storeViews and /rest/V1/store/storeConfigs both returned HTTP 401 {"message":"Missing Bearer token."} on 2026-09-05. A small directory subset is anonymous — GET /rest/V1/directory/countries returned HTTP 200.
  endpoint: https://store.safety-kleen.com/rest/
  header: Authorization
  id: commerce-rest-bearer
  scheme: bearer
  surface: Adobe Commerce REST
  type: http
  verified: probed
- description: Human web login only. No token endpoint, no OIDC discovery document (/.well-known/openid-configuration returned 404), and no documented programmatic access.
  endpoint: https://clhsaas.cleanharbors.com/
  id: chos-portal-login
  surface: Clean Harbors Online Services (CHOS) customer portal
  type: session
  verified: probed
slug: clean-harbors-authentication
source_filename: clean-harbors-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: >-\n  Derived on 2026-09-05 from graphql/clean-harbors-store-schema.graphql (introspected live\n  from https://store.safety-kleen.com/graphql) and from live unauthenticated calls against\n  https://store.safety-kleen.com/rest/ and https://careers.cleanharbors.com/api/mcp/jobs.\n  Clean Harbors publishes no developer authentication documentation, so nothing here is\n  quoted from the provider — every statement is an observation of a response we received.\nnote: >-\n  GraphQL has no securitySchemes block, so this profile is reconstructed from the schema's\n  own token mutations and from the status codes the endpoints actually returned.\nschemes:\n  - id: careers-anonymous\n    surface: Careers Job Query API\n    endpoint: https://careers.cleanharbors.com/api/mcp/jobs\n    type: none\n    description: >-\n      No credential of any kind. Every one of the four tools was called anonymously on\n      2026-09-05 and returned HTTP 200.\
  \ CORS is wide open\n      (access-control-allow-origin: *), so a browser-resident agent can call it directly.\n    verified: probed\n  - id: commerce-graphql-anonymous\n    surface: Clean Harbors / Safety-Kleen commerce GraphQL\n    endpoint: https://store.safety-kleen.com/graphql\n    type: none\n    description: >-\n      The catalog, CMS, store-configuration and guest-cart portion of the schema answers\n      with no credential. Full schema introspection is also anonymous and enabled — the\n      entire 861-type contract was read without a token.\n    verified: probed\n  - id: commerce-graphql-customer-token\n    surface: Clean Harbors / Safety-Kleen commerce GraphQL\n    endpoint: https://store.safety-kleen.com/graphql\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: 'Bearer <customer token>'\n    description: >-\n      Customer-scoped fields (customer, customerCart, customerOrders, company,\n      negotiableQuotes, requisition lists, purchase orders, wishlists)\
  \ require a customer\n      token. The schema issues one via the generateCustomerToken mutation and revokes it via\n      revokeCustomerToken; generateCustomerTokenAsAdmin exists for delegated impersonation.\n      There is no client-credentials, no OAuth authorization-code flow, and no\n      dynamic client registration in the contract.\n    token_mutations:\n      issue: generateCustomerToken\n      issue_delegated: generateCustomerTokenAsAdmin\n      revoke: revokeCustomerToken\n    verified: derived\n  - id: commerce-rest-bearer\n    surface: Adobe Commerce REST\n    endpoint: https://store.safety-kleen.com/rest/\n    type: http\n    scheme: bearer\n    header: Authorization\n    description: >-\n      Almost the whole REST surface is Bearer-gated. GET /rest/V1/store/storeViews and\n      /rest/V1/store/storeConfigs both returned HTTP 401 {\"message\":\"Missing Bearer token.\"}\n      on 2026-09-05. A small directory subset is anonymous —\n      GET /rest/V1/directory/countries returned\
  \ HTTP 200.\n    verified: probed\n  - id: chos-portal-login\n    surface: Clean Harbors Online Services (CHOS) customer portal\n    endpoint: https://clhsaas.cleanharbors.com/\n    type: session\n    description: >-\n      Human web login only. No token endpoint, no OIDC discovery document\n      (/.well-known/openid-configuration returned 404), and no documented programmatic access.\n    verified: probed\ndiscovery:\n  openid_configuration: not served on any Clean Harbors host (404 everywhere)\n  oauth_authorization_server: not served on any Clean Harbors host (404 everywhere)\n  oauth_protected_resource: not served on any Clean Harbors host (404 everywhere)\n  dynamic_client_registration: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clean-harbors/refs/heads/main/authentication/clean-harbors-authentication.yml
summary_line: 5 schemes
tags:
- Adobe Commerce
- Emergency Response
- Environmental Services
- Fortune 1000
- GraphQL
- Hazardous Waste
- Industrial Services
- Job Postings
- Manifest Tracking
- Recycling
- Remediation
---
