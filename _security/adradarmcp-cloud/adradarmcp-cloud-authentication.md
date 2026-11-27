---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AdRadar Authentication
name_suffix: Authentication
oauth_flows: []
overview: AdRadar declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AdRadar
provider_slug: adradarmcp-cloud
scheme_count: 2
schemes:
- authorizationUrl: https://accounts.google.com/o/oauth2/auth
  description: Google OAuth sign-in for Claude and ChatGPT clients
  flow: authorizationCode
  tokenUrl: https://oauth2.googleapis.com/token
  type: oauth2
- description: Bearer token provided after obtaining API key
  in: header
  name: Authorization
  type: apiKey
slug: adradarmcp-cloud-authentication
source_filename: adradarmcp-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://adradarmcp.cloud/en/setup/\nschemes:\n  - type: oauth2\n    description: Google OAuth sign-in for Claude and ChatGPT clients\n    flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token provided after obtaining API key\n"
source_yaml_url: https://artifacts.apis.io/adradarmcp-cloud/authentication/adradarmcp-cloud-authentication.yml
summary_line: 2 schemes
tags:
- AdTech
- Artificial Intelligence
- Advertising
- Meta
- TikTok
---
