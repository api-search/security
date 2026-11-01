---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pinboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinboard declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pinboard
provider_slug: pinboard
scheme_count: 2
schemes:
- description: Regular HTTP Auth (username/password) over HTTPS
  type: http
- description: API authentication token in the form username:TOKEN
  in: query
  name: auth_token
  type: apiKey
slug: pinboard-authentication
source_filename: pinboard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://pinboard.in/api/\nschemes:\n  - type: http\n    description: \"Regular HTTP Auth (username/password) over HTTPS\"\n  - type: apiKey\n    in: query\n    name: auth_token\n    description: \"API authentication token in the form username:TOKEN\"\n"
source_yaml_url: https://artifacts.apis.io/pinboard/authentication/pinboard-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Bookmarking
- Social
- API
- Productivity
- Web
---
