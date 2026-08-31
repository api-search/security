---
api_key_in:
- header
- query
api_specs:
- filename: electricity-north-west-catalog-api-openapi.yml
  format: yaml
  label: Electricity North West Catalog API
  slug: electricity-north-west-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/openapi/electricity-north-west-catalog-api-openapi.yml
- filename: electricity-north-west-dataset-api-openapi.yml
  format: yaml
  label: Electricity North West Dataset API
  slug: electricity-north-west-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/openapi/electricity-north-west-dataset-api-openapi.yml
auth_types:
- apiKey
- oauth2
- cookie
description: 'The OpenAPI documents declare a single scheme (an `apikey` query parameter), but that under-describes what the platform actually supports. The Opendatasoft (Huwise) Explore API accepts three credential styles — an API key in the Authorization header (the vendor''s recommended form), the same key as an `apikey` query parameter (the only one in the spec), and a portal session cookie — plus a full OAuth2 authorization-code flow for third-party applications. On the SP Electricity North West domain, catalogue and dataset METADATA is readable anonymously, but RECORD data is not: every dataset probed returned ForbiddenAccess to an unauthenticated caller.'
kind: authentication
layout: security
method: searched
name: Electricity North West Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Electricity North West secures its APIs with apiKey, oauth2, and cookie across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Electricity North West
provider_slug: electricity-north-west
scheme_count: 4
schemes:
- documented_only: true
  format: 'Authorization: Apikey <API_KEY>'
  in: header
  name: apikey (Authorization header)
  note: The vendor explicitly recommends the header over the query parameter because headers are not retained in browser history or server logs. This form is NOT declared in either OpenAPI document — a real gap between spec and docs.
  parameter: Authorization
  recommended: true
  sources:
  - https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication
  type: apiKey
- description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/electricity-north-west-explore-api-v2-0-openapi.json
  - openapi/electricity-north-west-explore-api-v2-1-openapi.json
  type: apiKey
- in: cookie
  name: portal session cookie
  note: Being logged in to the portal passes a session cookie with API calls, which is how the in-portal API console at /api-console/explore/v2.1/ authenticates.
  sources:
  - https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication
  type: cookie
- client_types:
  - confidential
  - public
  documented_only: true
  flows:
  - authorizationUrl: https://electricitynorthwest.opendatasoft.com/oauth2/authorize/
    flow: authorizationCode
    scopes:
      all: Full access on behalf of the authorizing user (the only scope supported)
    tokenUrl: https://electricitynorthwest.opendatasoft.com/oauth2/token/
  name: OAuth2
  probe:
    authorize_endpoint_status: 200 (redirects to /login/?next=/oauth2/authorize/)
    token_endpoint_status: 405 on GET (POST-only, as documented)
  registration: Applications are registered per domain from the "My applications" tab of the portal account page; registration yields a client_id and client_secret and requires a redirect URI.
  sources:
  - https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication
  standards:
  - RFC 6749
  - RFC 6750
  token_lifetime: The authorization code is 30 characters and must be exchanged within 1 hour. Bearer tokens expire and are renewed with a refresh token.
  type: oauth2
slug: electricity-north-west-authentication
source_filename: electricity-north-west-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Derived from openapi/electricity-north-west-explore-api-v2-0-openapi.json and\n  openapi/electricity-north-west-explore-api-v2-1-openapi.json, then upgraded from\n  the vendor authentication reference at\n  https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication and\n  live anonymous/gated probes of the electricitynorthwest domain on 2026-07-27.\ndocs: https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication\ndescription: >-\n  The OpenAPI documents declare a single scheme (an `apikey` query parameter),\n  but that under-describes what the platform actually supports. The Opendatasoft\n  (Huwise) Explore API accepts three credential styles — an API key in the\n  Authorization header (the vendor's recommended form), the same key as an\n  `apikey` query parameter (the only one in the spec), and a portal session\n  cookie — plus a full OAuth2 authorization-code flow for third-party\n  applications.\
  \ On the SP Electricity North West domain, catalogue and dataset\n  METADATA is readable anonymously, but RECORD data is not: every dataset probed\n  returned ForbiddenAccess to an unauthenticated caller.\nsummary:\n  types: [apiKey, oauth2, cookie]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode]\n  anonymous_access: partial\nschemes:\n- name: apikey (Authorization header)\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Apikey <API_KEY>'\n  recommended: true\n  documented_only: true\n  sources: [https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication]\n  note: >-\n    The vendor explicitly recommends the header over the query parameter because\n    headers are not retained in browser history or server logs. This form is NOT\n    declared in either OpenAPI document — a real gap between spec and docs.\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n\
  \  sources:\n  - openapi/electricity-north-west-explore-api-v2-0-openapi.json\n  - openapi/electricity-north-west-explore-api-v2-1-openapi.json\n- name: portal session cookie\n  type: cookie\n  in: cookie\n  note: >-\n    Being logged in to the portal passes a session cookie with API calls, which\n    is how the in-portal API console at /api-console/explore/v2.1/ authenticates.\n  sources: [https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://electricitynorthwest.opendatasoft.com/oauth2/authorize/\n    tokenUrl: https://electricitynorthwest.opendatasoft.com/oauth2/token/\n    scopes:\n      all: Full access on behalf of the authorizing user (the only scope supported)\n  standards: [RFC 6749, RFC 6750]\n  client_types: [confidential, public]\n  registration: >-\n    Applications are registered per domain from the \"My applications\" tab of the\n    portal account page;\
  \ registration yields a client_id and client_secret and\n    requires a redirect URI.\n  token_lifetime: >-\n    The authorization code is 30 characters and must be exchanged within 1 hour.\n    Bearer tokens expire and are renewed with a refresh token.\n  documented_only: true\n  probe:\n    authorize_endpoint_status: 200 (redirects to /login/?next=/oauth2/authorize/)\n    token_endpoint_status: 405 on GET (POST-only, as documented)\n  sources: [https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication]\nkey_management:\n  url: https://electricitynorthwest.opendatasoft.com/account/\n  page: My API keys tab of the portal account page\n  registration: https://electricitynorthwest.opendatasoft.com/pages/registration_log_in/\n  cost: free self-serve account\n  scoping: >-\n    By default an API key inherits the full rights of the user that created it,\n    so keys must not be shared. Per-key permissions can be narrowed through the\n    separate Automation API.\n  revocation:\
  \ Keys can be listed and revoked from the same account page.\naccess_observations:\n  generated: '2026-07-27'\n  anonymous_allowed:\n  - GET /api/explore/v2.1/catalog/datasets — 200, total_count 146\n  - GET /api/explore/v2.1/catalog/datasets/{dataset_id} — 200\n  - GET /api/explore/v2.1/catalog/facets — 200\n  - GET /api/explore/v2.1/catalog/exports — 200\n  - GET /api/explore/v2.1/catalog/exports/dcat — 200 (4.9 MB RDF/XML)\n  anonymous_denied:\n  - >-\n    GET /api/explore/v2.1/catalog/datasets/{dataset_id}/records — error_code\n    \"ForbiddenAccess\" on all five datasets probed (dfes-lv-headroom-monitored,\n    enwl_control_boundary, biodiversity-tree-opportunity, lv_load_duration,\n    enwl-lsoa-polygons). Several dataset descriptions state \"Actual dataset\n    content is available to registered users only\".\n  conclusion: >-\n    Metadata is open; record-level data requires a free registered account and an\n    API key. This is a registration wall, not a paywall.\nunauthorized_response:\n\
  \  status: 401\n  note: >-\n    Documented for private catalogs. In practice on this domain a missing\n    credential for record data surfaces as an error_code \"ForbiddenAccess\" body.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/authentication/electricity-north-west-authentication.yml
summary_line: apiKey/oauth2/cookie · 4 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- DER
- Renewables
- Energy Markets
- Smart Metering
---
