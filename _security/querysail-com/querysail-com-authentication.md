---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Querysail Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: querysail-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: querysail-com
provider_slug: querysail-com
scheme_count: 1
schemes:
- description: OAuth 2.1 with dynamic client registration for Google permissions.
  flows:
    authorizationCode:
      authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
      scopes:
        https://www.googleapis.com/auth/webmasters.readonly: Read‑only Search Console data
      tokenUrl: https://oauth2.googleapis.com/token
  type: oauth2
slug: querysail-com-authentication
source_filename: querysail-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://querysail.com/google-search-console\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 with dynamic client registration for Google permissions.\n    flows:\n      authorizationCode:\n        authorizationUrl: \"https://accounts.google.com/o/oauth2/v2/auth\"\n        tokenUrl: \"https://oauth2.googleapis.com/token\"\n        scopes:\n          \"https://www.googleapis.com/auth/webmasters.readonly\": \"Read‑only Search Console data\"\n"
source_yaml_url: https://artifacts.apis.io/querysail-com/authentication/querysail-com-authentication.yml
summary_line: 1 scheme
tags:
- MCP
- Google Search Console
- Google Analytics
- AI Assistants
- SaaS
---
