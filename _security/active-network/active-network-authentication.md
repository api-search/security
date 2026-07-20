---
api_key_in:
- query
api_specs:
- filename: active-network-activity-search-openapi.yml
  format: yaml
  label: ACTIVE Network Activity Search API v2
  slug: active-network-activity-search-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-network/refs/heads/main/openapi/active-network-activity-search-openapi.yml
- filename: active-network-campground-search-openapi.yml
  format: yaml
  label: ACTIVE Network Campground Search API
  slug: active-network-campground-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-network/refs/heads/main/openapi/active-network-campground-search-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Active Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Active Network secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Active Network
provider_slug: active-network
scheme_count: 1
schemes:
- description: API key passed as the api_key query parameter. Keys are issued via developer registration and are read-only.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  registration: https://developer.active.com/member/register
  sources:
  - openapi/active-network-activity-search-openapi.yml
  - openapi/active-network-campground-search-openapi.yml
  type: apiKey
slug: active-network-authentication
source_filename: active-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/active-network-activity-search-openapi.yml, openapi/active-network-campground-search-openapi.yml\ndocs: https://developer.active.com/docs/read/Activity_APIs\nnotes: >-\n  ACTIVE Network's public data APIs are read-only and, per the developer docs,\n  require no SSL or OAuth. Access is authenticated with a single API key passed\n  as the api_key query parameter, obtained by registering for a key at\n  https://developer.active.com/member/register.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as the api_key query parameter. Keys are issued via developer\n    registration and are read-only.\n  registration: https://developer.active.com/member/register\n  sources:\n  - openapi/active-network-activity-search-openapi.yml\n  - openapi/active-network-campground-search-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-network/refs/heads/main/authentication/active-network-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Events
- Registration
- Recreation
- Activities
- Sports
- Camping
- Search
- Ticketing
---
