---
api_key_in:
- query
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Swiftype Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swiftype secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Swiftype
provider_slug: swiftype
scheme_count: 2
schemes:
- access: read-write
  also_supports: HTTP Basic (username = auth_token, no password)
  description: Private API key (auth_token) granting full read/write access to all API operations for the account. Passed as an auth_token parameter, or via HTTP Basic auth using the key as the username with an empty password.
  in: query
  name: auth_token
  parameter: auth_token
  type: apiKey
- access: read-only
  description: Public, read-only engine key used for client-side / public search against a specific engine. Safe to expose in browser code; supports search and autocomplete only.
  in: query
  name: engine_key
  parameter: engine_key
  type: apiKey
slug: swiftype-authentication
source_filename: swiftype-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://swiftype.com/documentation/site-search/overview\ndocs: https://swiftype.com/documentation/site-search/overview\nsummary:\n  types: [apiKey, http]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  notes: >-\n    Swiftype Site Search authenticates with static credentials only. There is no\n    OAuth2/OIDC surface, so no scopes artifact applies.\nschemes:\n  - name: auth_token\n    type: apiKey\n    description: >-\n      Private API key (auth_token) granting full read/write access to all API\n      operations for the account. Passed as an auth_token parameter, or via HTTP\n      Basic auth using the key as the username with an empty password.\n    in: query\n    parameter: auth_token\n    also_supports: HTTP Basic (username = auth_token, no password)\n    access: read-write\n  - name: engine_key\n    type: apiKey\n    description: >-\n      Public, read-only engine key used for client-side / public search against\
  \ a\n      specific engine. Safe to expose in browser code; supports search and\n      autocomplete only.\n    in: query\n    parameter: engine_key\n    access: read-only\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftype/refs/heads/main/authentication/swiftype-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Search
- Site Search
- App Search
- Full Text Search
- Autocomplete
- Web Crawler
- Analytics
- Developer Tools
- Elastic
---
