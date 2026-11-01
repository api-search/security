---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sitesai Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: sitesai-net declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: sitesai-net
provider_slug: sitesai-net
scheme_count: 2
schemes:
- authorizationUrl: https://sitesai.net/oauth/authorize
  description: OAuth 2.1 with PKCE for user authentication.
  flow: authorizationCode
  scopes:
    intake: Limited intake-only access.
    read: Read access to data.
    write: Write access to data.
  tokenUrl: https://sitesai.net/oauth/token
  type: oauth2
- description: Personal API key for programmatic access.
  in: header
  name: X-API-Key
  type: apiKey
slug: sitesai-net-authentication
source_filename: sitesai-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: SitesAI authentication\ngenerated: '2026-10-30'\nmethod: searched\nsource: https://sitesai.net/llms.txt\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    description: OAuth 2.1 with PKCE for user authentication.\n    authorizationUrl: https://sitesai.net/oauth/authorize\n    tokenUrl: https://sitesai.net/oauth/token\n    scopes:\n      read: Read access to data.\n      write: Write access to data.\n      intake: Limited intake-only access.\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: Personal API key for programmatic access.\n"
source_yaml_url: https://artifacts.apis.io/sitesai-net/authentication/sitesai-net-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Construction
- Earthworks
- Estimating
- Field-Software
---
