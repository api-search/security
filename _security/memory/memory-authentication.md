---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Memory Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Memory secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Memory
provider_slug: memory
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.timelyapp.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.timelyapp.com/1.1/oauth/token
    tokenUrl_note: token URL inferred from the api.timelyapp.com/1.1 base and standard Timely OAuth layout; verify against the authenticated developer portal.
  name: OAuth2
  sources:
  - https://developer.timely.com/
  type: oauth2
slug: memory-authentication
source_filename: memory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.timely.com/\ndocs: https://developer.timely.com/\nnotes: >-\n  Timely's REST API (api.timelyapp.com/1.1) is secured with OAuth 2.0. The API\n  authorization endpoint https://api.timelyapp.com/1.1/oauth/authorize redirects\n  (HTTP 302) to https://app.timelyapp.com/oauth/authorize, confirming a\n  browser-based OAuth authorization flow; API requests are made with a bearer\n  access token. Exact token endpoint and scope list are documented behind the\n  authenticated developer portal (login via app.timelyapp.com/auth/docs) and are\n  not asserted here to avoid fabrication.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.timelyapp.com/oauth/authorize\n    tokenUrl: https://api.timelyapp.com/1.1/oauth/token\n    tokenUrl_note: >-\n      token URL inferred\
  \ from the api.timelyapp.com/1.1 base and standard Timely\n      OAuth layout; verify against the authenticated developer portal.\n  sources:\n  - https://developer.timely.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memory/refs/heads/main/authentication/memory-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Time Tracking
- Timesheets
- Productivity
- Project Management
- Professional Services
- Reporting
- Automation
- Artificial Intelligence
- SaaS
---
