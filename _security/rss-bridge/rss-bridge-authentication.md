---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Rss Bridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: RSS-Bridge declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: RSS-Bridge
provider_slug: rss-bridge
scheme_count: 3
schemes:
- description: HTTP Basic Authentication supported.
  scheme: basic
  type: http
- description: Token based authentication.
  in: query
  name: token
  type: apiKey
- description: Access control via web server configuration (nginx/caddy/apache).
  type: custom
slug: rss-bridge-authentication
source_filename: rss-bridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://raw.githubusercontent.com/RSS-Bridge/rss-bridge/master/docs/03_For_Hosts/06_Authentication.md\nschemes:\n  - type: http\n    scheme: basic\n    description: HTTP Basic Authentication supported.\n  - type: apiKey\n    name: token\n    in: query\n    description: Token based authentication.\n  - type: custom\n    description: Access control via web server configuration (nginx/caddy/apache).\n"
source_yaml_url: https://artifacts.apis.io/rss-bridge/authentication/rss-bridge-authentication.yml
summary_line: 3 schemes
tags:
- OpenSource
- PHP
- RSS
- Aggregator
- SelfHosted
---
