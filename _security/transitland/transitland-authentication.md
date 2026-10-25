---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: transitland-agencies-api-openapi.yml
  format: yaml
  label: TransitLand Agencies API
  slug: transitland-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-agencies-api-openapi.yml
- filename: transitland-feed-versions-api-openapi.yml
  format: yaml
  label: TransitLand Feed Versions API
  slug: transitland-feed-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-feed-versions-api-openapi.yml
- filename: transitland-feeds-api-openapi.yml
  format: yaml
  label: TransitLand Feeds API
  slug: transitland-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-feeds-api-openapi.yml
- filename: transitland-onestop-id-api-openapi.yml
  format: yaml
  label: TransitLand Onestop Id API
  slug: transitland-onestop-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-onestop-id-api-openapi.yml
- filename: transitland-operators-api-openapi.yml
  format: yaml
  label: TransitLand Operators API
  slug: transitland-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-operators-api-openapi.yml
- filename: transitland-routes-api-openapi.yml
  format: yaml
  label: TransitLand Routes API
  slug: transitland-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-routes-api-openapi.yml
- filename: transitland-stops-api-openapi.yml
  format: yaml
  label: TransitLand Stops API
  slug: transitland-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-stops-api-openapi.yml
- filename: transitland-street-routing-api-openapi.yml
  format: yaml
  label: TransitLand Street routing API
  slug: transitland-street-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-street-routing-api-openapi.yml
- filename: transitland-transit-routing-api-openapi.yml
  format: yaml
  label: TransitLand Transit routing API
  slug: transitland-transit-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-transit-routing-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Transitland Authentication
name_suffix: Authentication
oauth_flows: []
overview: TransitLand secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TransitLand
provider_slug: transitland
scheme_count: 2
schemes:
- description: API key sent as a request header. Preferred, since query strings are logged by intermediaries. `apikey`, `api_key`, `api_token`, and `access_token` are accepted equivalently, and headers may be spelled with a dash or an underscore.
  in: header
  name: apikeyHeader
  parameter: apikey
  sources:
  - openapi/transitland-routing-openapi.yml
  type: apiKey
- description: API key sent as a query parameter, for callers that cannot set headers. `apikey`, `api_key`, `api_token`, and `access_token` are accepted equivalently, and headers may be spelled with a dash or an underscore.
  in: query
  name: apikeyQuery
  parameter: apikey
  sources:
  - openapi/transitland-routing-openapi.yml
  type: apiKey
slug: transitland-authentication
source_filename: transitland-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/transitland-routing-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apikeyHeader\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key sent as a request header. Preferred, since query strings are logged by\n    intermediaries. `apikey`, `api_key`, `api_token`, and `access_token` are accepted equivalently,\n    and headers may be spelled with a dash or an underscore.\n  sources:\n  - openapi/transitland-routing-openapi.yml\n- name: apikeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key sent as a query parameter, for callers that cannot set headers. `apikey`,\n    `api_key`, `api_token`, and `access_token` are accepted equivalently, and headers may be\n    spelled with a dash or an underscore.\n  sources:\n  - openapi/transitland-routing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/authentication/transitland-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Transportation
- Public APIs
- Transit
- GTFS
- Open Data
- Routing
- Geospatial
---
