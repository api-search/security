---
api_key_in:
- query
- header
api_specs:
- filename: endeavour-energy-catalog-api-openapi.yml
  format: yaml
  label: Endeavour Energy Catalog API
  slug: endeavour-energy-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavour-energy/refs/heads/main/openapi/endeavour-energy-catalog-api-openapi.yml
- filename: endeavour-energy-dataset-api-openapi.yml
  format: yaml
  label: Endeavour Energy Dataset API
  slug: endeavour-energy-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavour-energy/refs/heads/main/openapi/endeavour-energy-dataset-api-openapi.yml
auth_types:
- none
- apiKey
- oauth2
description: 'The Explore API is anonymous by default. Every one of the eight published datasets answers HTTP 200 with no credential of any kind — no signup, no key, no licence click-through. The OpenAPI contract declares exactly one security scheme (an apiKey in the query string), but that understates the platform: the docs and the live host also support an Authorization header form, portal session cookies, and a full OAuth2 authorization-code flow. The spec is thin; this profile is the superset.'
kind: authentication
layout: security
method: searched
name: Endeavour Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Endeavour Energy secures its APIs with none, apiKey, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Endeavour Energy
provider_slug: endeavour-energy
scheme_count: 5
schemes:
- declared_in_spec: false
  detail: 'The default and the recommended path for this provider. Verified 2026-07-27: GET /api/explore/v2.1/catalog/datasets -> 200 (total_count 8) and GET /api/explore/v2.1/catalog/datasets/outagecustomerlive/records?limit=1 -> 200, both with no Authorization header and no apikey parameter.'
  name: anonymous
  quota: 5000 calls/day (X-RateLimit-Limit observed)
  type: none
- declared_in_spec: true
  description: API key to make authenticated requests.
  in: query
  name: apikey
  note: The only scheme the contract declares, and the one the docs advise AGAINST — query strings are retained in browser history and server logs.
  parameter: apikey
  recommended: false
  sources:
  - openapi/endeavour-energy-open-data-explore-api-v2-0-openapi.json
  - openapi/endeavour-energy-open-data-explore-api-v2-1-openapi.json
  type: apiKey
- declared_in_spec: false
  format: 'Authorization: Apikey <API_KEY>'
  in: header
  name: apikey-header
  note: Documented and supported, but absent from the OpenAPI contract. A client generated purely from the spec will use the discouraged query form.
  parameter: Authorization
  recommended: true
  type: apiKey
- declared_in_spec: false
  detail: Being logged into https://data.endeavourenergy.com.au/ passes a session cookie along with API calls, authenticating the user for the request.
  login: https://data.endeavourenergy.com.au/login/
  name: portal-session
  type: cookie
- client_types:
  - confidential
  - public
  declared_in_spec: false
  detail: The Opendatasoft platform implements a full OAuth2 authorization-code flow so a third party can query data on a user's behalf without handling their password. Applications are registered per domain from the account page and can only access data on that domain.
  detail_file: scopes/endeavour-energy-scopes.yml
  flows:
  - authorizationUrl: https://data.endeavourenergy.com.au/oauth2/authorize/
    flow: authorizationCode
    scope_names:
    - all
    scopes: 1
    tokenUrl: https://data.endeavourenergy.com.au/oauth2/token/
  name: oauth2
  rfc:
  - RFC 6749
  - RFC 6750
  token_type: Bearer
  type: oauth2
  verified_live:
  - note: endpoint exists; redirects to login
    status: 302
    url: https://data.endeavourenergy.com.au/oauth2/authorize/
  - note: endpoint exists; POST-only
    status: 405
    url: https://data.endeavourenergy.com.au/oauth2/token/
slug: endeavour-energy-authentication
source_filename: endeavour-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  openapi/endeavour-energy-open-data-explore-api-v2-1-openapi.json,\n  openapi/endeavour-energy-open-data-explore-api-v2-0-openapi.json (declared\n  securitySchemes), upgraded with\n  https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html#section/Authentication\n  and live anonymous probes of https://data.endeavourenergy.com.au on\n  2026-07-27.\ndocs: 'https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html#section/Authentication'\ndescription: >-\n  The Explore API is anonymous by default. Every one of the eight published\n  datasets answers HTTP 200 with no credential of any kind — no signup, no key,\n  no licence click-through. The OpenAPI contract declares exactly one security\n  scheme (an apiKey in the query string), but that understates the platform:\n  the docs and the live host also support an Authorization header form, portal\n  session cookies, and a full OAuth2 authorization-code flow.\
  \ The spec is thin;\n  this profile is the superset.\n\nsummary:\n  types: [none, apiKey, oauth2]\n  api_key_in: [query, header]\n  oauth2_flows: [authorizationCode]\n  anonymous_access: true\n  credential_required: false\n\nschemes:\n  - name: anonymous\n    type: none\n    declared_in_spec: false\n    detail: >-\n      The default and the recommended path for this provider. Verified 2026-07-27:\n      GET /api/explore/v2.1/catalog/datasets -> 200 (total_count 8) and\n      GET /api/explore/v2.1/catalog/datasets/outagecustomerlive/records?limit=1\n      -> 200, both with no Authorization header and no apikey parameter.\n    quota: 5000 calls/day (X-RateLimit-Limit observed)\n\n  - name: apikey\n    type: apiKey\n    in: query\n    parameter: apikey\n    declared_in_spec: true\n    description: API key to make authenticated requests.\n    sources:\n      - openapi/endeavour-energy-open-data-explore-api-v2-0-openapi.json\n      - openapi/endeavour-energy-open-data-explore-api-v2-1-openapi.json\n\
  \    recommended: false\n    note: >-\n      The only scheme the contract declares, and the one the docs advise\n      AGAINST — query strings are retained in browser history and server logs.\n\n  - name: apikey-header\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Apikey <API_KEY>'\n    declared_in_spec: false\n    recommended: true\n    note: >-\n      Documented and supported, but absent from the OpenAPI contract. A client\n      generated purely from the spec will use the discouraged query form.\n\n  - name: portal-session\n    type: cookie\n    declared_in_spec: false\n    detail: >-\n      Being logged into https://data.endeavourenergy.com.au/ passes a session\n      cookie along with API calls, authenticating the user for the request.\n    login: https://data.endeavourenergy.com.au/login/\n\n  - name: oauth2\n    type: oauth2\n    declared_in_spec: false\n    rfc: [RFC 6749, RFC 6750]\n    flows:\n      - flow: authorizationCode\n  \
  \      authorizationUrl: https://data.endeavourenergy.com.au/oauth2/authorize/\n        tokenUrl: https://data.endeavourenergy.com.au/oauth2/token/\n        scopes: 1\n        scope_names: [all]\n    token_type: Bearer\n    client_types: [confidential, public]\n    detail: >-\n      The Opendatasoft platform implements a full OAuth2 authorization-code\n      flow so a third party can query data on a user's behalf without handling\n      their password. Applications are registered per domain from the account\n      page and can only access data on that domain.\n    verified_live:\n      - {url: 'https://data.endeavourenergy.com.au/oauth2/authorize/', status: 302, note: 'endpoint exists; redirects to login'}\n      - {url: 'https://data.endeavourenergy.com.au/oauth2/token/', status: 405, note: 'endpoint exists; POST-only'}\n    detail_file: scopes/endeavour-energy-scopes.yml\n\nkey_provisioning:\n  url: https://data.endeavourenergy.com.au/account/\n  path: '\"My API keys\" tab on the account\
  \ page'\n  self_serve: false\n  note: >-\n    https://data.endeavourenergy.com.au/signup/ 302-redirects to the portal\n    home — open self-serve registration is not enabled on this domain, and\n    /account/api-keys/ redirects to /login/. Since every dataset is public and\n    anonymous, this limits quota, not access.\n  key_scope_warning: >-\n    Published caveat: \"By default, every API key authenticates requests as\n    coming from your user, which means they grant the same rights (yours) to\n    any person using them.\" Keys are user-scoped, not application-scoped,\n    unless narrowed through the Automation API.\n\nnot_present:\n  openid_connect: 'GET /.well-known/openid-configuration -> 404 on both hosts'\n  oauth_metadata: 'GET /.well-known/oauth-authorization-server -> 404 on both hosts (the OAuth2 surface exists but is not advertised via RFC 8414 discovery)'\n  mutual_tls: false\n  http_basic: 'Only at the OAuth2 token endpoint, to pass client_id/client_secret.'\n\nout_of_band:\n\
  \  csip_aus_utility_server: >-\n    Endeavour Energy operates a CSIP-AUS (IEEE 2030.5 / SEP2 derivative)\n    utility server for NSW flexible exports and the emergency backstop\n    mechanism. CSIP-AUS conventionally uses mutual TLS with device\n    certificates, but Endeavour Energy publishes no endpoint, no security\n    scheme and no onboarding path for it, so no auth model is asserted here.\n    Onboarding runs through CEC-approved inverter equipment and a connectivity\n    capability test in the NSW CER Installer Portal at installation time.\n\nrelated:\n  - scopes/endeavour-energy-scopes.yml\n  - conventions/endeavour-energy-conventions.yml\n  - well-known/endeavour-energy-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavour-energy/refs/heads/main/authentication/endeavour-energy-authentication.yml
summary_line: none/apiKey/oauth2 · 5 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Open Data
- Energy Networks
- Distribution
- Outages
- Consumer Data Right
- Smart Metering
- DER
- Solar
- Renewables
---
