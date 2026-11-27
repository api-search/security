---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Japan Startup Resources Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Japan Startup Resources secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Japan Startup Resources
provider_slug: japanstartupresources-com
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://japanstartupresources.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://japanstartupresources.com/oauth/token
  name: subscriberOAuth
  sources:
  - openapi/japanstartupresources-com-openapi.json
  type: oauth2
slug: japanstartupresources-com-authentication
source_filename: japanstartupresources-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/japanstartupresources-com-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: subscriberOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://japanstartupresources.com/oauth/authorize\n    tokenUrl: https://japanstartupresources.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/japanstartupresources-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/japanstartupresources-com/authentication/japanstartupresources-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Startups
- Japan
- Entrepreneurship
- Directory
- Newsletters
---
