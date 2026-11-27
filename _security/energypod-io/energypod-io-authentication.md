---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: EnergyPod Authentication
name_suffix: Authentication
oauth_flows: []
overview: EnergyPod declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EnergyPod
provider_slug: energypod-io
scheme_count: 2
schemes:
- description: API key format epk_<id>.<secret>
  scheme: bearer
  type: http
- authorizationUrl: https://energypod.io/oauth/authorize
  flow: authorization_code
  scopes:
    read: Read access to MCP tools
  tokenUrl: https://energypod.io/oauth/token
  type: oauth2
slug: energypod-io-authentication
source_filename: energypod-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://energypod.io/mcp/docs#oauth\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"API key format epk_<id>.<secret>\"\n  - type: oauth2\n    flow: authorization_code\n    authorizationUrl: https://energypod.io/oauth/authorize\n    tokenUrl: https://energypod.io/oauth/token\n    scopes:\n      read: \"Read access to MCP tools\""
source_yaml_url: https://artifacts.apis.io/energypod-io/authentication/energypod-io-authentication.yml
summary_line: 2 schemes
tags:
- Energy
- Podcasts
- Artificial Intelligence
- Weekly
- Media
---
