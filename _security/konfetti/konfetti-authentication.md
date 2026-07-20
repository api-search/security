---
api_key_in: []
api_specs:
- filename: konfetti-store-openapi.yml
  format: yaml
  label: konfetti Store API
  slug: store
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-store-openapi.yml
auth_types:
- none
- http
- oauth2
description: 'How authentication works on the konfetti Store API. Three postures coexist: the /v1/store/* catalog is fully public, /v1/checkout/* and /v1/user/* require a Bearer access token, and tokens are issued by an OAuth 2.0 token endpoint that has no publicly documented client-registration path.'
kind: authentication
layout: security
method: derived
name: Konfetti Authentication
name_suffix: Authentication
oauth_flows: []
overview: konfetti secures its APIs with none, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: konfetti
provider_slug: konfetti
scheme_count: 3
schemes:
- applies_to:
  - GET /v1/store/events
  - GET /v1/store/events/{permalink}
  - GET /v1/store/events/{permalink}/similar
  - GET /v1/store/categories
  - GET /v1/categories
  description: The entire /v1/store/* catalog surface — events, event detail, similar events, categories, and /v1/categories — answered HTTP 200 with no credentials at all. This is an unauthenticated public read API in practice, though konfetti does not describe it as one and publishes no terms covering its use.
  name: none
  sources:
  - live probe 2026-07-19
  type: none
- applies_to:
  - GET /v1/user/profile
  - GET /v1/checkout/orders
  description: '''Authorization: Bearer <access_token>''. The first-party client obtains a token, then sends it on every protected call alongside ''Content-Type: application/json''.'
  failure_mode: A missing or expired token produces HTTP 302 redirecting to https://api.gokonfetti.com/login — NOT a 401. Clients must disable redirect-following on API calls or they will parse an HTML login page as JSON.
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/konfetti-store-openapi.yml
  - live probe 2026-07-19
  type: http
- description: 'A standard OAuth 2.0 token endpoint, confirmed by probing: an empty POST returned HTTP 400 with the League OAuth2 Server error envelope {"error":"unsupported_grant_type","error_description":"The authorization grant type is not supported by the authorization server.","hint":"Check that all required parameters have been provided"}. League OAuth2 Server is the library behind Laravel Passport, which is consistent with the Apiato/Laravel stack serving the API.'
  flows: []
  name: oauth2
  not_published:
  - authorization endpoint
  - supported grant types
  - client registration process
  - scope reference (no scopes are declared anywhere)
  - RFC 8414 authorization server metadata (/.well-known/oauth-authorization-server returns 404)
  - PKCE or device-authorization guidance
  observed:
    empty_post_status: 400
    error_family: RFC 6749 section 5.2
    get_status: 405
  sources:
  - openapi/konfetti-store-openapi.yml
  - live probe 2026-07-19
  token_endpoint: https://api.gokonfetti.com/v1/oauth/token
  type: oauth2
slug: konfetti-authentication
source_filename: konfetti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: >-\n  openapi/konfetti-store-openapi.yml, plus live probes of\n  https://api.gokonfetti.com/v1 on 2026-07-19 and the Authorization-header\n  handling in the publicly served gokonfetti.com Nuxt bundles. konfetti\n  publishes no authentication documentation, so this profile is observed\n  behaviour rather than a provider reference.\ndescription: >-\n  How authentication works on the konfetti Store API. Three postures coexist:\n  the /v1/store/* catalog is fully public, /v1/checkout/* and /v1/user/* require\n  a Bearer access token, and tokens are issued by an OAuth 2.0 token endpoint\n  that has no publicly documented client-registration path.\n\nsummary:\n  types:\n  - none\n  - http\n  - oauth2\n  public_read: true\n  third_party_access: >-\n    Not available. The OAuth 2.0 token endpoint is live but konfetti publishes\n    no client registration, no grant-type list, no scope reference and no\n    RFC 8414 metadata, so there\
  \ is no documented route for a third party to\n    obtain credentials.\n\nschemes:\n- name: none\n  type: none\n  description: >-\n    The entire /v1/store/* catalog surface — events, event detail, similar\n    events, categories, and /v1/categories — answered HTTP 200 with no\n    credentials at all. This is an unauthenticated public read API in practice,\n    though konfetti does not describe it as one and publishes no terms covering\n    its use.\n  applies_to:\n  - GET /v1/store/events\n  - GET /v1/store/events/{permalink}\n  - GET /v1/store/events/{permalink}/similar\n  - GET /v1/store/categories\n  - GET /v1/categories\n  sources:\n  - live probe 2026-07-19\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: >-\n    'Authorization: Bearer <access_token>'. The first-party client obtains a\n    token, then sends it on every protected call alongside\n    'Content-Type: application/json'.\n  applies_to:\n  - GET /v1/user/profile\n\
  \  - GET /v1/checkout/orders\n  failure_mode: >-\n    A missing or expired token produces HTTP 302 redirecting to\n    https://api.gokonfetti.com/login — NOT a 401. Clients must disable\n    redirect-following on API calls or they will parse an HTML login page as\n    JSON.\n  sources:\n  - openapi/konfetti-store-openapi.yml\n  - live probe 2026-07-19\n- name: oauth2\n  type: oauth2\n  token_endpoint: https://api.gokonfetti.com/v1/oauth/token\n  flows: []\n  description: >-\n    A standard OAuth 2.0 token endpoint, confirmed by probing: an empty POST\n    returned HTTP 400 with the League OAuth2 Server error envelope\n    {\"error\":\"unsupported_grant_type\",\"error_description\":\"The authorization\n    grant type is not supported by the authorization server.\",\"hint\":\"Check\n    that all required parameters have been provided\"}. League OAuth2 Server is\n    the library behind Laravel Passport, which is consistent with the\n    Apiato/Laravel stack serving the API.\n  observed:\n\
  \    get_status: 405\n    empty_post_status: 400\n    error_family: RFC 6749 section 5.2\n  not_published:\n  - authorization endpoint\n  - supported grant types\n  - client registration process\n  - scope reference (no scopes are declared anywhere)\n  - RFC 8414 authorization server metadata (/.well-known/oauth-authorization-server returns 404)\n  - PKCE or device-authorization guidance\n  sources:\n  - openapi/konfetti-store-openapi.yml\n  - live probe 2026-07-19\n\naccount_creation:\n  endpoint: POST /v1/register\n  required_fields: [email, password, first_name]\n  evidence: >-\n    Probing with an empty body returned HTTP 422 naming exactly these three\n    required fields, in the request locale.\n  note: >-\n    This creates a consumer account for the marketplace, not an API client\n    credential. Partner (supplier) accounts are provisioned by konfetti through\n    the partner sign-up flow and used at backoffice.gokonfetti.com.\n\ntransport_security:\n  tls: TLSv1.3 on api.gokonfetti.com\n\
  \  hsts: false\n  detail: security/konfetti-domain-security.yml\n\ngaps:\n- No 401 on authentication failure — a 302 HTML redirect is returned instead.\n- No scopes, so tokens cannot be least-privileged.\n- No token introspection or revocation endpoint published.\n- No API key alternative for server-to-server use.\n- No RFC 8414 or OpenID Connect discovery document.\n\nrelated:\n  openapi: openapi/konfetti-store-openapi.yml\n  conventions: conventions/konfetti-conventions.yml\n  errors: errors/konfetti-problem-types.yml\n  well_known: well-known/konfetti-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/authentication/konfetti-authentication.yml
summary_line: none/http/oauth2 · 3 schemes
tags:
- Company
- Marketplace
- Experiences
- Booking
- Events
- Workshops
- Ticketing
- Gift Cards
- Travel and Leisure
- Germany
- Commerce
---
