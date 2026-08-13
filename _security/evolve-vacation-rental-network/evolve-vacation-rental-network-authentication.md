---
api_key_in: []
auth_types: []
description: 'Evolve publishes no developer program, no API reference and no OpenAPI, so there is no securityScheme block to derive an auth profile from. What this file records is what an anonymous probe could actually observe: one live OpenID Connect provider on an Evolve-controlled host, and two credentialed API surfaces whose auth mechanism is visible only from the outside.'
kind: authentication
layout: security
method: probed
name: Evolve Vacation Rental Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evolve declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Evolve
provider_slug: evolve-vacation-rental-network
scheme_count: 0
schemes: []
slug: evolve-vacation-rental-network-authentication
source_filename: evolve-vacation-rental-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://help.evolve.com/.well-known/openid-configuration\nname: Evolve — authentication profile\ndescription: >-\n  Evolve publishes no developer program, no API reference and no OpenAPI, so there is\n  no securityScheme block to derive an auth profile from. What this file records is\n  what an anonymous probe could actually observe: one live OpenID Connect provider on\n  an Evolve-controlled host, and two credentialed API surfaces whose auth mechanism is\n  visible only from the outside.\nderived_from_openapi: false\nopenapi_present: false\nproviders:\n- id: help-evolve-oidc\n  name: Evolve Help Center identity provider\n  type: openIdConnect\n  host: help.evolve.com\n  issuer: https://help.evolve.com\n  discovery: https://help.evolve.com/.well-known/openid-configuration\n  status: 200\n  ownership_note: >-\n    issuer and every advertised endpoint resolve to help.evolve.com, an Evolve-owned\n    hostname, so the tenant is Evolve's.\
  \ The endpoint layout (/services/oauth2/*,\n    /id/keys, /services/data) is Salesforce Experience Cloud's standard shape — this\n    is Evolve's Salesforce community, not an API product Evolve designed.\n  endpoints:\n    authorization: https://help.evolve.com/services/oauth2/authorize\n    token: https://help.evolve.com/services/oauth2/token\n    revocation: https://help.evolve.com/services/oauth2/revoke\n    introspection: https://help.evolve.com/services/oauth2/introspect\n    userinfo: https://help.evolve.com/services/oauth2/userinfo\n    registration: https://help.evolve.com/services/oauth2/register\n    end_session: https://help.evolve.com/services/auth/idp/oidc/logout\n    jwks: https://help.evolve.com/id/keys\n  jwks_status: 200\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n\
  \  - public\n  scopes_supported_count: 36\n  scopes: scopes/evolve-vacation-rental-network-scopes.yml\n  claims_supported_count: 24\n  dynamic_client_registration: true\n  dynamic_client_registration_note: >-\n    A /services/oauth2/register endpoint is advertised. Advertised is not the same as\n    open — it was not exercised, and Salesforce gates it on a connected-app policy.\n  pkce_advertised: false\n  pkce_note: >-\n    code_challenge_methods_supported is absent from the discovery document. Salesforce\n    supports PKCE regardless; the omission is a discovery-document gap, not proof PKCE\n    is unavailable.\nobserved_gated_surfaces:\n- id: api-evolve-com\n  host: api.evolve.com\n  url: https://api.evolve.com/\n  status: 403\n  mechanism: unknown\n  evidence: >-\n    AWS API Gateway (x-amz-apigw-id, x-amzn-errortype ForbiddenException) behind\n    Cloudflare. Every probed path returns {\"message\":\"Forbidden\"} with no\n    WWW-Authenticate header, so the credential type is not disclosed\
  \ to anonymous\n    callers. No authorizer challenge, no OAuth metadata.\n- id: owner-evolve-graphql\n  host: owner.evolve.com\n  url: https://owner.evolve.com/graphql\n  status: 307\n  mechanism: session-cookie\n  evidence: >-\n    POST of a GraphQL introspection query returns 307 to\n    /login/idp?redirect_url=%2Fgraphql — the owner portal's identity provider. The\n    endpoint is real and session-gated; the schema is not introspectable anonymously.\nsummary:\n  schemes_documented_by_provider: 0\n  schemes_observed: 1\n  oauth2: true\n  openid_connect: true\n  api_key: null\n  mutual_tls: null\n  note: >-\n    api_key and mutual_tls are null, not false — Evolve documents nothing, so their\n    absence is unmeasured rather than measured.\ndocs: null\ndocs_note: >-\n  Searched evolve.com, owner.evolve.com, help.evolve.com and the licensed-partners\n  page for an authentication or developer page. None exists.\nchecked: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolve-vacation-rental-network/refs/heads/main/authentication/evolve-vacation-rental-network-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Travel
- Hospitality
- Vacation Rentals
- Short-Term Rentals
- Property Management
- Real Estate
- Booking
---
