---
api_key_in:
- header
api_specs:
- filename: rocketreach-people-lookup-api-openapi.yml
  format: yaml
  label: RocketReach People Lookup API
  slug: rocketreach-people-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-lookup-api-openapi.yml
- filename: rocketreach-people-search-api-openapi.yml
  format: yaml
  label: RocketReach People Search API
  slug: rocketreach-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-search-api-openapi.yml
- filename: rocketreach-company-lookup-api-openapi.yml
  format: yaml
  label: RocketReach Company Lookup API
  slug: rocketreach-company-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-lookup-api-openapi.yml
- filename: rocketreach-company-search-api-openapi.yml
  format: yaml
  label: RocketReach Company Search API
  slug: rocketreach-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-search-api-openapi.yml
- filename: rocketreach-account-api-openapi.yml
  format: yaml
  label: RocketReach Account API
  slug: rocketreach-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-account-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rocketreach Authentication
name_suffix: Authentication
oauth_flows: []
overview: RocketReach secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RocketReach
provider_slug: rocketreach
scheme_count: 1
schemes:
- description: RocketReach account API key. You can locate your API Key from the "My API Key" section of the [API account page](https://rocketreach.co/account?section=nav_gen_api). Requests to the API are authenticated using the Api-Key request header. Older clients may use an `api_key` query parameter, but this behavior is deprecated.
  in: header
  name: RocketReachAPIKey
  parameter: Api-Key
  sources:
  - openapi/rocketreach-account-api-openapi.yml
  - openapi/rocketreach-company-lookup-api-openapi.yml
  - openapi/rocketreach-company-search-api-openapi.yml
  - openapi/rocketreach-people-lookup-api-openapi.yml
  - openapi/rocketreach-people-search-api-openapi.yml
  type: apiKey
slug: rocketreach-authentication
source_filename: rocketreach-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rocketreach-account-api-openapi.yml, openapi/rocketreach-company-lookup-api-openapi.yml,\n  openapi/rocketreach-company-search-api-openapi.yml, openapi/rocketreach-people-lookup-api-openapi.yml,\n  openapi/rocketreach-people-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RocketReachAPIKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: RocketReach account API key. You can locate your API Key from the \"My API Key\"\n    section of the [API account page](https://rocketreach.co/account?section=nav_gen_api). Requests\n    to the API are authenticated using the Api-Key request header. Older clients may use an\n    `api_key` query parameter, but this behavior is deprecated.\n  sources:\n  - openapi/rocketreach-account-api-openapi.yml\n  - openapi/rocketreach-company-lookup-api-openapi.yml\n  - openapi/rocketreach-company-search-api-openapi.yml\n  -\
  \ openapi/rocketreach-people-lookup-api-openapi.yml\n  - openapi/rocketreach-people-search-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/authentication/rocketreach-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B
- Contact Data
- Email Lookup
- Phone Lookup
- Sales Intelligence
- Lead Generation
- People Search
- Company Search
- Data Enrichment
- Prospecting
- Recruiting
- Webhooks
---
