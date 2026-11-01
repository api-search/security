---
anonymous_access: false
api_key_in: []
api_specs:
- filename: housingfeed-com-sample-api-openapi.yml
  format: yaml
  label: housingfeed-com Sample API
  slug: housingfeed-com-sample-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/housingfeed-com/openapi/housingfeed-com-sample-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Housingfeed Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: housingfeed-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: housingfeed-com
provider_slug: housingfeed-com
scheme_count: 2
schemes:
- description: Apify API token for Data API (also accepted as Bearer Authorization header)
  in: query
  name: token
  type: apiKey
- description: Bearer token issued with a Display Feed licence for Feed API
  scheme: bearer
  type: http
slug: housingfeed-com-authentication
source_filename: housingfeed-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://housingfeed.com/docs/authentication\nschemes:\n  - type: apiKey\n    name: token\n    in: query\n    description: Apify API token for Data API (also accepted as Bearer Authorization header)\n  - type: http\n    scheme: bearer\n    description: Bearer token issued with a Display Feed licence for Feed API\n"
source_yaml_url: https://artifacts.apis.io/housingfeed-com/authentication/housingfeed-com-authentication.yml
summary_line: 2 schemes
tags:
- RealEstate
- Rentals
- DataAPI
- US
- Listings
---
