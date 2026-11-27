---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Everloot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everloot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Everloot
provider_slug: everloot-app
scheme_count: 1
schemes:
- description: Optional API key for higher rate limits
  in: header
  name: X-API-Key
  type: apiKey
slug: everloot-app-authentication
source_filename: everloot-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: https://everloot.app/docs/api\nschemes:\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: Optional API key for higher rate limits"
source_yaml_url: https://artifacts.apis.io/everloot-app/authentication/everloot-app-authentication.yml
summary_line: 1 scheme
tags:
- Gaming
- WoW
- Database
- GuildTracker
- Tools
---
