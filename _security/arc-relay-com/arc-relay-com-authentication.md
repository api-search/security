---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ARC-Relay Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARC-Relay declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ARC-Relay
provider_slug: arc-relay-com
scheme_count: 3
schemes:
- description: Bearer token with prefix ar_agent_ for agent keys
  in: header
  name: Authorization
  type: apiKey
- description: Pass agent key directly via X-Api-Key header
  in: header
  name: X-Api-Key
  type: apiKey
- description: Bearer token with prefix ar_live_ for user keys (manage account)
  in: header
  name: Authorization
  type: apiKey
slug: arc-relay-com-authentication
source_filename: arc-relay-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://arc-relay.com/developers.html\nname: ARC-Relay Authentication\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token with prefix ar_agent_ for agent keys\"\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: \"Pass agent key directly via X-Api-Key header\"\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token with prefix ar_live_ for user keys (manage account)\"\n"
source_yaml_url: https://artifacts.apis.io/arc-relay-com/authentication/arc-relay-com-authentication.yml
summary_line: 3 schemes
tags:
- Email
- Forwarding
- SRS
- Arc
- Services
---
