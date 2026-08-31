---
api_key_in:
- query
- header
api_specs:
- filename: scottishpower-catalog-api-openapi.yml
  format: yaml
  label: ScottishPower Catalog API
  slug: scottishpower-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scottishpower/refs/heads/main/openapi/scottishpower-catalog-api-openapi.yml
- filename: scottishpower-dataset-api-openapi.yml
  format: yaml
  label: ScottishPower Dataset API
  slug: scottishpower-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scottishpower/refs/heads/main/openapi/scottishpower-dataset-api-openapi.yml
auth_types:
- apiKey
description: 'The auth profile for ScottishPower''s only public API. Derived from the OpenAPI securityScheme, then upgraded from the Opendatasoft Explore API authentication documentation and live probes on 2026-07-27. The headline is that authentication is optional: the catalogue and a subset of dataset records are readable with no key and no account at all.'
kind: authentication
layout: security
method: searched
name: Scottishpower Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScottishPower secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ScottishPower
provider_slug: scottishpower
scheme_count: 2
schemes:
- description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/scottishpower-spen-open-data-explore-api-openapi.json
  type: apiKey
- description: The form the Opendatasoft docs recommend over the query parameter, because headers are not stored in browser history or server logs. Not present in the harvested securitySchemes — a real gap between the published contract and the documented behaviour.
  format: 'Authorization: Apikey <API_KEY>'
  in: header
  name: Authorization header (documented, not declared in the spec)
  parameter: Authorization
  sources:
  - https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication
  type: apiKey
slug: scottishpower-authentication
source_filename: scottishpower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/scottishpower-spen-open-data-explore-api-openapi.json\ndocs: https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication\ndescription: >-\n  The auth profile for ScottishPower's only public API. Derived from the OpenAPI\n  securityScheme, then upgraded from the Opendatasoft Explore API authentication\n  documentation and live probes on 2026-07-27. The headline is that\n  authentication is optional: the catalogue and a subset of dataset records are\n  readable with no key and no account at all.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - header\n  oauth2_flows: []\n  required: false\n  anonymous_access: true\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n  sources:\n  - openapi/scottishpower-spen-open-data-explore-api-openapi.json\n- name: Authorization header (documented, not declared in the spec)\n\
  \  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Apikey <API_KEY>'\n  description: >-\n    The form the Opendatasoft docs recommend over the query parameter, because\n    headers are not stored in browser history or server logs. Not present in the\n    harvested securitySchemes — a real gap between the published contract and the\n    documented behaviour.\n  sources:\n  - https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication\nanonymous:\n  verified: '2026-07-27'\n  evidence: >-\n    GET /api/explore/v2.1/catalog/datasets returned HTTP 200 with total_count 150\n    and no credentials of any kind. A bogus key returns HTTP 401\n    {\"error\": \"API key is not valid\"} — so supplying a bad key is worse than\n    supplying none.\n  scope: >-\n    Catalogue metadata for all 150 datasets. Record-level access is not uniformly\n    anonymous — 87 of 100 datasets probed returned HTTP 403 ForbiddenAccess on\n    /records. See errors/scottishpower-problem-types.yml.\n\
  keys:\n  self_serve: true\n  url: https://spenergynetworks.opendatasoft.com/account/api-keys/\n  signup: https://spenergynetworks.opendatasoft.com/signup/\n  login: https://spenergynetworks.opendatasoft.com/login/\n  benefit: Extended quotas and access to datasets granted to the account.\noauth2:\n  available_on_this_domain: false\n  platform_capability: true\n  standards: [RFC 6749, RFC 6750]\n  probes:\n    - {url: 'https://spenergynetworks.opendatasoft.com/api/oauth2/authorize', http_status: 404, date: '2026-07-27'}\n    - {url: 'https://spenergynetworks.opendatasoft.com/api/oauth2/token', http_status: 404, date: '2026-07-27'}\n  note: >-\n    Opendatasoft documents an OAuth2 authorization-code flow with bearer tokens\n    for third-party applications registered on a domain, but no OAuth2 endpoint\n    responds on the SP Energy Networks domain. No scopes/ artifact is emitted,\n    because there is no OAuth surface to enumerate.\noidc:\n  discovery: false\n  note: /.well-known/openid-configuration\
  \ returns 404 on the API host.\nconsumer_side:\n  note: >-\n    ScottishPower Energy Retail exposes no authenticated customer API. There is a\n    conventional web/app account login at www.scottishpower.co.uk, but that host\n    returns HTTP 403 to every anonymous client and documents no token endpoint,\n    no OAuth flow and no third-party data-access path. Britain has no consumer\n    energy data right that would require one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scottishpower/refs/heads/main/authentication/scottishpower-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Retailer
- Smart Metering
- Grid
- Open Data
- Distribution Network Operator
- Renewables
- Energy Markets
---
