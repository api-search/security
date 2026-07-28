---
api_key_in:
- query
- header
api_specs:
- filename: northern-powergrid-open-data-explore-api-v2-1-openapi.json
  format: json
  label: Northern Powergrid Open Data Explore API
  slug: northern-powergrid-open-data-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/openapi/northern-powergrid-open-data-explore-api-v2-1-openapi.json
- filename: northern-powergrid-open-data-explore-api-v2-0-openapi.json
  format: json
  label: Northern Powergrid Open Data Explore API v2.0
  slug: northern-powergrid-open-data-explore-api-v2-0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/openapi/northern-powergrid-open-data-explore-api-v2-0-openapi.json
auth_types:
- none
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Northern Powergrid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Northern Powergrid secures its APIs with none, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Northern Powergrid
provider_slug: northern-powergrid
scheme_count: 4
schemes:
- description: No credential required. The catalogue, dataset metadata, facets and the records of the datasets Northern Powergrid publishes openly all answer to unauthenticated callers, subject to the anonymous daily quota. Roughly 44 of the 102 datasets are metadata-visible but records-gated and return no rows to anonymous callers.
  name: anonymous
  sources:
  - live probe 2026-07-27
  type: none
- description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/northern-powergrid-open-data-explore-api-v2-0-openapi.json
  - openapi/northern-powergrid-open-data-explore-api-v2-1-openapi.json
  type: apiKey
- description: The platform's recommended way to pass the API key, documented but absent from the OpenAPI. Preferred over the query parameter because headers are not retained in browser history or server logs.
  format: 'Authorization: Apikey <API_KEY>'
  in: header
  name: apikey-header
  parameter: Authorization
  recommended: true
  scheme: Apikey
  sources:
  - https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Providing-API-keys-within-requests
  type: http
- description: OAuth 2.0 authorization-code flow for third-party applications acting on behalf of a portal user. RFC 6749 compliant, bearer tokens per RFC 6750. Applications are registered per domain from the account "My applications" tab; authorization codes expire after 1 hour and are exchanged for a bearer token plus a refresh token.
  flows:
  - authorizationUrl: https://northernpowergrid.opendatasoft.com/oauth2/authorize/
    client_types:
    - confidential
    - public
    flow: authorizationCode
    refresh: true
    scopes:
    - all
    tokenUrl: https://northernpowergrid.opendatasoft.com/oauth2/token/
  name: oauth2
  sources:
  - https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Using-OAuth2-authorization
  - live probe 2026-07-27
  type: oauth2
slug: northern-powergrid-authentication
source_filename: northern-powergrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/northern-powergrid-open-data-explore-api-v2-0-openapi.json, openapi/northern-powergrid-open-data-explore-api-v2-1-openapi.json\ndocs: https://help.huwise.com/apis/ods-explore-v2/#section/Authentication\nnote: >-\n  The OpenAPI declares only the apikey query-parameter scheme. The platform's own reference\n  documentation for this API documents two further mechanisms the spec omits: the same API key\n  passed in an Authorization header (the vendor's recommended form), and a full OAuth 2.0\n  authorization-code flow with refresh tokens. Both were verified live against this portal on\n  2026-07-27 — GET /oauth2/authorize/ returned 302 and POST-only /oauth2/token/ returned 405 to a\n  GET. Anonymous access needs no credential at all: the catalogue and most datasets answer\n  unauthenticated at 5,000 requests a day.\nsummary:\n  types:\n  - none\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  - header\n  oauth2_flows:\n\
  \  - authorizationCode\n  anonymous_access: true\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    No credential required. The catalogue, dataset metadata, facets and the records of the datasets\n    Northern Powergrid publishes openly all answer to unauthenticated callers, subject to the\n    anonymous daily quota. Roughly 44 of the 102 datasets are metadata-visible but records-gated and\n    return no rows to anonymous callers.\n  sources:\n  - live probe 2026-07-27\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n  sources:\n  - openapi/northern-powergrid-open-data-explore-api-v2-0-openapi.json\n  - openapi/northern-powergrid-open-data-explore-api-v2-1-openapi.json\n- name: apikey-header\n  type: http\n  scheme: Apikey\n  in: header\n  parameter: Authorization\n  format: \"Authorization: Apikey <API_KEY>\"\n  description: >-\n    The platform's recommended way to pass the API key, documented but\
  \ absent from the OpenAPI.\n    Preferred over the query parameter because headers are not retained in browser history or\n    server logs.\n  recommended: true\n  sources:\n  - https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Providing-API-keys-within-requests\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code flow for third-party applications acting on behalf of a portal user.\n    RFC 6749 compliant, bearer tokens per RFC 6750. Applications are registered per domain from the\n    account \"My applications\" tab; authorization codes expire after 1 hour and are exchanged for a\n    bearer token plus a refresh token.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://northernpowergrid.opendatasoft.com/oauth2/authorize/\n    tokenUrl: https://northernpowergrid.opendatasoft.com/oauth2/token/\n    refresh: true\n    client_types: [confidential, public]\n    scopes: [all]\n  sources:\n  - https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Using-OAuth2-authorization\n\
  \  - live probe 2026-07-27\ncredential_acquisition:\n  signup: https://northernpowergrid.opendatasoft.com/signup/\n  login: https://northernpowergrid.opendatasoft.com/account/login/\n  cost: free\n  effect: >-\n    A free portal account raises the daily API allowance above the anonymous 5,000 and unlocks the\n    records of the datasets that are hidden from anonymous callers.\nrelated:\n  scopes: scopes/northern-powergrid-scopes.yml\n  conventions: conventions/northern-powergrid-conventions.yml\n  rate_limits: rate-limits/northern-powergrid-rate-limits.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/authentication/northern-powergrid-authentication.yml
summary_line: none/apiKey/oauth2 · 4 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Open Data
- Distribution Network Operator
- Smart Metering
- Network Capacity
- Flexibility
- DER
- Renewables
---
