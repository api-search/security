---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Airship Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Airship secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Airship
provider_slug: airship
scheme_count: 3
schemes:
- description: HTTP Basic auth using app_key and app_secret (App level).
  name: BasicAppAuth
  scheme: basic
  sources:
  - openapi/airship-openapi.yml
  type: http
- description: Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/airship-openapi.yml
  type: http
- description: 'OAuth 2.0 scoped tokens. Scopes include att (attachments), chn (channels),

    cnt (contacts), evt (events), lst (lists), nu (named users), pln (pipelines),

    psh (push), rpt (reports), sch (schedules), tpl (content templates).'
  flows:
  - flow: clientCredentials
    scopes: 11
    tokenUrl: https://oauth2.asnapieu.com/token
  name: OAuth2
  sources:
  - openapi/airship-openapi.yml
  type: oauth2
slug: airship-authentication
source_filename: airship-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airship-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BasicAppAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using app_key and app_secret (App level).\n  sources:\n  - openapi/airship-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token.\n  sources:\n  - openapi/airship-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth2.asnapieu.com/token\n    scopes: 11\n  description: |-\n    OAuth 2.0 scoped tokens. Scopes include att (attachments), chn (channels),\n    cnt (contacts), evt (events), lst (lists), nu (named users), pln (pipelines),\n    psh (push), rpt (reports), sch (schedules), tpl (content templates).\n  sources:\n  - openapi/airship-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/authentication/airship-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Notifications
- Push
- Email
- Mobile
- CDP
---
