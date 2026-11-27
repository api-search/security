---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fabricate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fabricate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fabricate
provider_slug: fabricate-build
scheme_count: 1
schemes:
- flows:
    authorizationCode:
      authorizationUrl: https://fabricate.build/oauth/authorize
      scopes:
        fabricate:read: Read owned app titles, statuses and subscription tier
      tokenUrl: https://fabricate.build/oauth/token
  name: agentOAuth
  type: oauth2
slug: fabricate-build-authentication
source_filename: fabricate-build-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: https://fabricate.build/openapi.json\nschemes:\n  - type: oauth2\n    name: agentOAuth\n    flows:\n      authorizationCode:\n        authorizationUrl: https://fabricate.build/oauth/authorize\n        tokenUrl: https://fabricate.build/oauth/token\n        scopes:\n          fabricate:read: Read owned app titles, statuses and subscription tier\n"
source_yaml_url: https://artifacts.apis.io/fabricate-build/authentication/fabricate-build-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- No-Code
- App Builder
- Cloudflare
- Web Development
---
