---
api_key_in:
- header
api_specs:
- filename: monday-com-webhooks-asyncapi.yml
  format: yaml
  label: Monday.com API
  slug: monday-com
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/monday-com/refs/heads/main/asyncapi/monday-com-webhooks-asyncapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Monday Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Monday.com secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Monday.com
provider_slug: monday-com
scheme_count: 2
schemes:
- description: 'Personal API token from the monday.com developer settings, passed as

    the `Authorization` header value (no `Bearer` prefix).'
  in: header
  name: apiToken
  parameter: Authorization
  sources:
  - openapi/monday-com-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://auth.monday.com/oauth2/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://auth.monday.com/oauth2/token
  name: oauth2
  sources:
  - openapi/monday-com-openapi.yml
  type: oauth2
slug: monday-com-authentication
source_filename: monday-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/monday-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Personal API token from the monday.com developer settings, passed as\n    the `Authorization` header value (no `Bearer` prefix).\n  sources:\n  - openapi/monday-com-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.monday.com/oauth2/authorize\n    tokenUrl: https://auth.monday.com/oauth2/token\n    scopes: 7\n  sources:\n  - openapi/monday-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monday-com/refs/heads/main/authentication/monday-com-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Work Management
- CRM
- Automation
- GraphQL
---
