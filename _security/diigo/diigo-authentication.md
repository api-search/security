---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Diigo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diigo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Diigo
provider_slug: diigo
scheme_count: 2
schemes:
- description: API key required as query parameter.
  in: query
  name: api_key
  type: apiKey
- description: HTTP Basic authentication with base64 encoded username and password.
  scheme: basic
  type: http
slug: diigo-authentication
source_filename: diigo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: searched\nsource: https://www.diigo.com/api_dev\nschemes:\n  - type: apiKey\n    name: api_key\n    in: query\n    description: API key required as query parameter.\n  - type: http\n    scheme: basic\n    description: HTTP Basic authentication with base64 encoded username and password.\n"
source_yaml_url: https://artifacts.apis.io/diigo/authentication/diigo-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
