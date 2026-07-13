---
api_key_in: []
api_specs:
- filename: stack-exchange-openapi.yml
  format: yaml
  label: Stack Exchange API
  slug: stack-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Stack Exchange Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Stack Exchange secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Stack Exchange
provider_slug: stack-exchange
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication for Stack Exchange API. Register an application at http://stackapps.com/apps/oauth to obtain client credentials.
  flows:
  - authorizationUrl: https://stackoverflow.com/oauth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://stackoverflow.com/oauth/access_token/json
  name: oauth2
  sources:
  - openapi/stack-exchange-openapi.yml
  type: oauth2
slug: stack-exchange-authentication
source_filename: stack-exchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stack-exchange-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://stackoverflow.com/oauth\n    tokenUrl: https://stackoverflow.com/oauth/access_token/json\n    scopes: 3\n  description: OAuth 2.0 authentication for Stack Exchange API. Register an application at http://stackapps.com/apps/oauth\n    to obtain client credentials.\n  sources:\n  - openapi/stack-exchange-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/authentication/stack-exchange-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Answers
- Code
- Community
- Developer Tools
- Knowledge Base
- Q&A
- Questions
- Stack Exchange
---
