---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Eurolytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eurolytics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Eurolytics
provider_slug: eurolytics-app
scheme_count: 2
schemes:
- description: Bearer el_... (API key)
  in: header
  name: Authorization
  type: apiKey
- description: Bearer elat_... (OAuth 2.1 access token)
  flows:
    authorizationCode:
      authorizationUrl: https://eurolytics.app/oauth/authorize
      scopes: {}
      tokenUrl: https://eurolytics.app/oauth/token
  type: oauth2
slug: eurolytics-app-authentication
source_filename: eurolytics-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://eurolytics.app/docs/install.json\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer el_... (API key)\"\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://eurolytics.app/oauth/authorize\n        tokenUrl: https://eurolytics.app/oauth/token\n        scopes: {}\n    description: \"Bearer elat_... (OAuth 2.1 access token)\"\n"
source_yaml_url: https://artifacts.apis.io/eurolytics-app/authentication/eurolytics-app-authentication.yml
summary_line: 2 schemes
tags:
- Analytics
- Privacy
- GDPR
- Web Analytics
- EU-hosted
---
