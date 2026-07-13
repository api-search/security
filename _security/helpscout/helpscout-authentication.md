---
api_key_in: []
api_specs:
- filename: helpscout-openapi.yml
  format: yaml
  label: Help Scout Conversations API
  slug: helpscout-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-openapi.yml
- filename: helpscout-webhooks-asyncapi.yml
  format: yaml
  label: Help Scout Webhooks API
  slug: helpscout-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/asyncapi/helpscout-webhooks-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Helpscout Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Help Scout secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Help Scout
provider_slug: helpscout
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  sources:
  - openapi/helpscout-openapi.yml
  type: oauth2
slug: helpscout-authentication
source_filename: helpscout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/helpscout-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/helpscout-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/authentication/helpscout-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Customer Support
- Help Desk
- Email
- Live Chat
- Knowledge Base
- SaaS
---
