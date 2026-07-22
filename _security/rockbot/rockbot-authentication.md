---
api_key_in: []
api_specs:
- filename: rockbot-openapi.yml
  format: yaml
  label: Rockbot API
  slug: rockbot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Rockbot Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Rockbot secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Rockbot
provider_slug: rockbot
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Client Credentials grant. Exchange a CLIENT_ID/CLIENT_SECRET (issued by Rockbot support) at the token endpoint for a 24-hour bearer ACCESS_TOKEN, then send it as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.rockbot.com/v5/api-clients/token
  name: oauth2
  sources:
  - openapi/rockbot-openapi.yml
  type: oauth2
slug: rockbot-authentication
source_filename: rockbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rockbot-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.rockbot.com/v5/api-clients/token\n    scopes: 0\n  description: 'OAuth 2.0 Client Credentials grant. Exchange a CLIENT_ID/CLIENT_SECRET (issued\n    by Rockbot support) at the token endpoint for a 24-hour bearer ACCESS_TOKEN, then send it\n    as `Authorization: Bearer ACCESS_TOKEN`.'\n  sources:\n  - openapi/rockbot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/authentication/rockbot-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Music
- Digital Signage
- Audio Messaging
- Retail Media
- In-Location Media
- Media
- Entertainment
---
