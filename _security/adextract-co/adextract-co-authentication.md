---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: adextract Authentication
name_suffix: Authentication
oauth_flows: []
overview: adextract declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: adextract
provider_slug: adextract-co
scheme_count: 2
schemes:
- description: API key generated from account page.
  in: header
  name: X-API-Key
  type: apiKey
- description: OAuth flow for agents.
  flows:
    authorizationCode:
      authorizationUrl: https://adextract.co/oauth/authorize
      scopes: {}
      tokenUrl: https://adextract.co/oauth/token
  type: oauth2
slug: adextract-co-authentication
source_filename: adextract-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://adextract.co/documentation\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key generated from account page.\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://adextract.co/oauth/authorize\n        tokenUrl: https://adextract.co/oauth/token\n        scopes: {}\n    description: OAuth flow for agents.\n"
source_yaml_url: https://artifacts.apis.io/adextract-co/authentication/adextract-co-authentication.yml
summary_line: 2 schemes
tags:
- Advertising
- Artificial Intelligence
- MCP
- Marketing
- Competitor Analysis
---
