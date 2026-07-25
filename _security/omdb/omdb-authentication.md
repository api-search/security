---
api_key_in:
- query
api_specs:
- filename: omdb-id-parameter-api-openapi.yml
  format: yaml
  label: OMDb ID Parameter API
  slug: omdb-id-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omdb/refs/heads/main/openapi/omdb-id-parameter-api-openapi.yml
- filename: omdb-search-parameter-api-openapi.yml
  format: yaml
  label: OMDb Search Parameter API
  slug: omdb-search-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omdb/refs/heads/main/openapi/omdb-search-parameter-api-openapi.yml
- filename: omdb-title-parameter-api-openapi.yml
  format: yaml
  label: OMDb Title Parameter API
  slug: omdb-title-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omdb/refs/heads/main/openapi/omdb-title-parameter-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Omdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: OMDb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OMDb
provider_slug: omdb
scheme_count: 1
schemes:
- description: API key obtained from https://www.omdbapi.com/apikey.aspx
  in: query
  name: APIKeyQueryParam
  parameter: apikey
  sources:
  - openapi/omdb-api-openapi.yml
  type: apiKey
slug: omdb-authentication
source_filename: omdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/omdb-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: APIKeyQueryParam\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key obtained from https://www.omdbapi.com/apikey.aspx\n  sources:\n  - openapi/omdb-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omdb/refs/heads/main/authentication/omdb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Movies
- Television
- Entertainment
- Metadata
- Ratings
- Posters
- IMDb
- Open Data
---
