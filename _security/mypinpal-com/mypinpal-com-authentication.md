---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mypinpal Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: mypinpal-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mypinpal-com
provider_slug: mypinpal-com
scheme_count: 1
schemes:
- authorizationUrl: https://notes.mypinpal.com/oauth/authorize
  flow: authorizationCode
  scopes:
    notes: Access notes data
  tokenUrl: https://notes.mypinpal.com/oauth/token
  type: oauth2
slug: mypinpal-com-authentication
source_filename: mypinpal-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://mypinpal.com/notes/api\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://notes.mypinpal.com/oauth/authorize\n    tokenUrl: https://notes.mypinpal.com/oauth/token\n    scopes:\n      notes: Access notes data\n"
source_yaml_url: https://artifacts.apis.io/mypinpal-com/authentication/mypinpal-com-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Productivity
- Notes
- Projects
- Sweden
---
