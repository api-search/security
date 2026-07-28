---
api_key_in:
- query
api_specs:
- filename: uk-power-networks-explore-api-v2-1-openapi.json
  format: json
  label: UK Power Networks Open Data Explore API v2.1
  slug: uk-power-networks-explore-api-v2-1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/openapi/uk-power-networks-explore-api-v2-1-openapi.json
- filename: uk-power-networks-explore-api-v2-0-openapi.json
  format: json
  label: UK Power Networks Open Data Explore API v2.0
  slug: uk-power-networks-explore-api-v2-0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/openapi/uk-power-networks-explore-api-v2-0-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Uk Power Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: UK Power Networks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UK Power Networks
provider_slug: uk-power-networks
scheme_count: 1
schemes:
- applied: global (spec-level security requirement on both the v2.0 and v2.1 documents)
  description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/uk-power-networks-explore-api-v2-0-openapi.json
  - openapi/uk-power-networks-explore-api-v2-1-openapi.json
  type: apiKey
slug: uk-power-networks-authentication
source_filename: uk-power-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/uk-power-networks-explore-api-v2-0-openapi.json, openapi/uk-power-networks-explore-api-v2-1-openapi.json\ndocs: https://ukpowernetworks.opendatasoft.com/account/api-keys/\ndocs_secondary:\n- https://ukpn-dso.github.io/ukpyn/getting-started/\n- https://github.com/UKPN-DSO/ukpyn\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2: false\n  oidc: false\n  mtls: false\n  accreditation: false\nmodel: >-\n  A single API key passed as an apikey query-string parameter. There is no OAuth 2.0, no OpenID\n  Connect, no mutual TLS and no accreditation regime — /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server both return HTTP 404 on the API host. Because the key\n  travels in the query string rather than an Authorization header it will appear in server logs,\n  browser history and Referer headers; treat it as a low-sensitivity read credential and rotate it\n  from the account page\
  \ rather than embedding it in shared URLs.\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n  applied: global (spec-level security requirement on both the v2.0 and v2.1 documents)\n  sources:\n  - openapi/uk-power-networks-explore-api-v2-0-openapi.json\n  - openapi/uk-power-networks-explore-api-v2-1-openapi.json\nanonymous_access:\n  supported: true\n  scope: >-\n    The whole catalogue surface answers anonymously — dataset listing, dataset metadata, facets and\n    the DCAT-AP export. Records answer anonymously for 36 of the 136 catalogued datasets; the other\n    99 return HTTP 403 ForbiddenAccess until a key is supplied. Verified 2026-07-27 by enumerating\n    every dataset_id and issuing an anonymous records call against each.\n  rate_limit: 10000 calls per day (x-ratelimit-limit header on an anonymous 200)\nonboarding:\n  gate: self-serve\n  approval_required: false\n  cost: free\n  steps:\n  - Create\
  \ a free account at https://ukpowernetworks.opendatasoft.com/signup/\n  - Sign in and open https://ukpowernetworks.opendatasoft.com/account/api-keys/\n  - Generate a key\n  - Pass it on every call as the apikey query parameter\n  sdk_convention: >-\n    The official Python client (ukpyn) reads the key from a UKPN_API_KEY environment variable or a\n    .env file rather than taking it inline.\nevidence:\n- source: openapi securitySchemes (both documents)\n  value: '{\"apikey\": {\"type\": \"apiKey\", \"name\": \"apikey\", \"in\": \"query\"}}'\n- source: https://ukpowernetworks.opendatasoft.com/account/api-keys/\n  http_status: 200\n  fetched: '2026-07-27'\n  note: Redirects to /login/?next=/account/api-keys/ when unauthenticated.\n- source: https://ukpowernetworks.opendatasoft.com/.well-known/openid-configuration\n  http_status: 404\n  fetched: '2026-07-27'\n- source: https://ukpowernetworks.opendatasoft.com/.well-known/oauth-authorization-server\n  http_status: 404\n  fetched: '2026-07-27'\n\
  related:\n  scopes: null\n  conventions: conventions/uk-power-networks-conventions.yml\n  well_known: well-known/uk-power-networks-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/authentication/uk-power-networks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- Smart Metering
- DER
- EV Charging
- Carbon
- Energy Markets
---
