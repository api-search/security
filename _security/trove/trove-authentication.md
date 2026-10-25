---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: trove-contributor-api-openapi.yml
  format: yaml
  label: Trove Contributor API
  slug: trove-contributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-contributor-api-openapi.yml
- filename: trove-list-api-openapi.yml
  format: yaml
  label: Trove List API
  slug: trove-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-list-api-openapi.yml
- filename: trove-newspaper-api-openapi.yml
  format: yaml
  label: Trove Newspaper API
  slug: trove-newspaper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-newspaper-api-openapi.yml
- filename: trove-people-api-openapi.yml
  format: yaml
  label: Trove People API
  slug: trove-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-people-api-openapi.yml
- filename: trove-search-api-openapi.yml
  format: yaml
  label: Trove Search API
  slug: trove-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-search-api-openapi.yml
- filename: trove-work-api-openapi.yml
  format: yaml
  label: Trove Work API
  slug: trove-work-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-work-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Trove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trove secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trove
provider_slug: trove
scheme_count: 2
schemes:
- description: Enter your Trove API key to execute a call
  in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/trove-openapi.yml
  type: apiKey
- description: 'Docs examples pass the key as a query parameter: https://api.trove.nla.gov.au/v3/result?key=<INSERT KEY>&category=<CATEGORY NAME>&q=<YOUR SEARCH TERMS>'
  in: query
  name: key (query)
  parameter: key
  sources:
  - https://trove.nla.gov.au/about/create-something/using-api/v3/api-technical-guide
  type: apiKey
slug: trove-authentication
source_filename: trove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://trove.nla.gov.au/about/create-something/using-api/v3/api-technical-guide\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Enter your Trove API key to execute a call\n  sources:\n  - openapi/trove-openapi.yml\n- name: key (query)\n  type: apiKey\n  in: query\n  parameter: key\n  description: 'Docs examples pass the key as a query parameter: https://api.trove.nla.gov.au/v3/result?key=<INSERT\n    KEY>&category=<CATEGORY NAME>&q=<YOUR SEARCH TERMS>'\n  sources:\n  - https://trove.nla.gov.au/about/create-something/using-api/v3/api-technical-guide\ndocs: https://trove.nla.gov.au/about/create-something/using-api\ndocs_pages:\n- https://trove.nla.gov.au/about/create-something/using-api\n- https://trove.nla.gov.au/about/create-something/using-api/v3/api-technical-guide\nkey_issuance:\n  text: You will need a\
  \ Trove account to receive a Trove API key.\n  process: Request a Trove API key form; applications reviewed at Levels 1-4, most\n    answered within a week. Since 2025-05-15 keys are allocated by review rather than\n    automatically.\n  key_types: A Full text-type API key is required to receive full text (since 2026-05-27).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/authentication/trove-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- News
- Public APIs
- Libraries
- Cultural Heritage
- Digitised Newspapers
- Archives
- Open Data
- Australia
- Search
---
