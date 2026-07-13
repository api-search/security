---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Zoho Mail API
  slug: zoho-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-mail/refs/heads/main/openapi/openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho Mail Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoho Mail secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoho Mail
provider_slug: zoho-mail
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: OAuth2
  sources:
  - openapi/openapi.json
  type: oauth2
slug: zoho-mail-authentication
source_filename: zoho-mail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 11\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-mail/refs/heads/main/authentication/zoho-mail-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Email
- Mail
- Collaboration
- Messaging
- Calendar
- Contacts
- Organization Management
- SaaS
---
