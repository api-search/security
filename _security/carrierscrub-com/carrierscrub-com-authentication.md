---
anonymous_access: false
api_key_in: []
api_specs:
- filename: carrierscrub-com-authority-history-api-openapi.yml
  format: yaml
  label: CarrierScrub Authority History API
  slug: carrierscrub-com-authority-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrierscrub-com/openapi/carrierscrub-com-authority-history-api-openapi.yml
- filename: carrierscrub-com-batch-api-openapi.yml
  format: yaml
  label: CarrierScrub Batch API
  slug: carrierscrub-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrierscrub-com/openapi/carrierscrub-com-batch-api-openapi.yml
- filename: carrierscrub-com-fmcsa-activity-api-openapi.yml
  format: yaml
  label: CarrierScrub Fmcsa Activity API
  slug: carrierscrub-com-fmcsa-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrierscrub-com/openapi/carrierscrub-com-fmcsa-activity-api-openapi.yml
- filename: carrierscrub-com-lookup-api-openapi.yml
  format: yaml
  label: CarrierScrub Lookup API
  slug: carrierscrub-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrierscrub-com/openapi/carrierscrub-com-lookup-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: CarrierScrub Authentication
name_suffix: Authentication
oauth_flows: []
overview: CarrierScrub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CarrierScrub
provider_slug: carrierscrub-com
scheme_count: 1
schemes:
- description: 'Authorization: Bearer cs_live_... An owner or admin of the brokerage, on any plan, creates keys in Admin, then API keys. A key that goes unused for 60 days stops working.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/carrierscrub-com-openapi.json
  type: http
slug: carrierscrub-com-authentication
source_filename: carrierscrub-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/carrierscrub-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer cs_live_... An owner or admin of the brokerage, on any\n    plan, creates keys in Admin, then API keys. A key that goes unused for 60 days stops working.'\n  sources:\n  - openapi/carrierscrub-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/carrierscrub-com/authentication/carrierscrub-com-authentication.yml
summary_line: http · 1 scheme
tags:
- carrier-vetting
- Freight Brokerage
- FMCSA Data
---
