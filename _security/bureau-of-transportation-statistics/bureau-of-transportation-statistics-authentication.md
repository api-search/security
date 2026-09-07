---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: bureau-of-transportation-statistics-metadata-api-openapi.yml
  format: yaml
  label: Bureau of Transportation Statistics Metadata API
  slug: bureau-of-transportation-statistics-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-transportation-statistics/refs/heads/main/openapi/bureau-of-transportation-statistics-metadata-api-openapi.yml
- filename: bureau-of-transportation-statistics-resource-api-openapi.yml
  format: yaml
  label: Bureau of Transportation Statistics Resource API
  slug: bureau-of-transportation-statistics-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-transportation-statistics/refs/heads/main/openapi/bureau-of-transportation-statistics-resource-api-openapi.yml
- filename: bureau-of-transportation-statistics-geodata-search-openapi.json
  format: json
  label: BTS Geospatial Search API (NTAD)
  slug: bts-geospatial-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-transportation-statistics/refs/heads/main/openapi/bureau-of-transportation-statistics-geodata-search-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bureau Of Transportation Statistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Transportation Statistics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bureau of Transportation Statistics
provider_slug: bureau-of-transportation-statistics
scheme_count: 2
schemes:
- description: Socrata application token from data.bts.gov developer registration.
  docs: https://dev.socrata.com/docs/app-tokens.html
  in: header
  name: appToken
  parameter: X-App-Token
  registration: https://data.bts.gov/profile/edit/developer_settings
  required: false
  sources:
  - openapi/bureau-of-transportation-statistics-resource-api-openapi.yml
  - openapi/bureau-of-transportation-statistics-metadata-api-openapi.yml
  type: apiKey
- description: The same application token passed as a query parameter, for clients that cannot set a custom header (e.g. a browser fetch from a static page).
  in: query
  name: appTokenQuery
  parameter: $$app_token
  required: false
  sources:
  - openapi/bureau-of-transportation-statistics-resource-api-openapi.yml
  type: apiKey
slug: bureau-of-transportation-statistics-authentication
source_filename: bureau-of-transportation-statistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/bureau-of-transportation-statistics-resource-api-openapi.yml\ndocs: https://dev.socrata.com/docs/app-tokens.html\nregistration: https://data.bts.gov/profile/edit/developer_settings\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  required: false\n  anonymous_access: true\nnote: >-\n  EVERY BTS API SURFACE READS ANONYMOUSLY. There is no OAuth, no OIDC, no bearer token and\n  no signup gate on the data — /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server return 404 on data.bts.gov, geodata.bts.gov and\n  www.transtats.bts.gov (see well-known/). The one credential that exists, the Socrata\n  application token, is not an access grant: the platform documentation states that\n  untokened requests \"come from a shared pool via IP address\" subject to throttling, while\n  tokened requests are \"not throttled ... unless those requests are determined to be\n  abusive or malicious\"\
  . Register free, send it on every call, and expect nothing else\n  from it.\nschemes:\n- name: appToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  description: Socrata application token from data.bts.gov developer registration.\n  required: false\n  registration: https://data.bts.gov/profile/edit/developer_settings\n  docs: https://dev.socrata.com/docs/app-tokens.html\n  sources:\n  - openapi/bureau-of-transportation-statistics-resource-api-openapi.yml\n  - openapi/bureau-of-transportation-statistics-metadata-api-openapi.yml\n- name: appTokenQuery\n  type: apiKey\n  in: query\n  parameter: $$app_token\n  description: >-\n    The same application token passed as a query parameter, for clients that cannot set a\n    custom header (e.g. a browser fetch from a static page).\n  required: false\n  sources:\n  - openapi/bureau-of-transportation-statistics-resource-api-openapi.yml\nsurfaces:\n- host: data.bts.gov\n  auth: optional-api-key\n  scheme: appToken\n  verified: >-\n \
  \   GET https://data.bts.gov/resource/bw6n-ddqk.json?$limit=2 returned HTTP 200 with no\n    credential, 2026-09-05.\n- host: geodata.bts.gov\n  auth: none\n  scheme: null\n  verified: >-\n    GET https://geodata.bts.gov/api/search/v1/conformance and\n    /api/search/definition/?f=json both returned HTTP 200 anonymously, 2026-09-05. The\n    published OpenAPI declares no securitySchemes. Individual operations accept an optional\n    `token` query parameter for ArcGIS-secured items only.\n- host: services.arcgis.com/xOi1kZaI0eWDREZv\n  auth: optional-token\n  scheme: arcgis-token\n  verified: >-\n    GET .../arcgis/rest/info?f=json returns\n    authInfo.isTokenBasedSecurity true with tokenServicesUrl\n    https://www.arcgis.com/sharing/generateToken — this governs private items in the USDOT\n    ArcGIS Online tenant; the NTAD feature services referenced from geodata.bts.gov are\n    public and read without a token.\n- host: www.transtats.bts.gov\n  auth: none\n  scheme: null\n  verified:\
  \ >-\n    HTML query forms only, no machine-readable contract and no credential (HTTP 200,\n    2026-09-05).\noauth: false\nscopes: false\nscopes_note: >-\n  No scopes/ artifact is written: there is no OAuth surface anywhere on this provider, so\n  there is nothing to scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-transportation-statistics/refs/heads/main/authentication/bureau-of-transportation-statistics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal-Government
- Statistics
- Transportation
- Aviation
- Freight
- Open Data
---
