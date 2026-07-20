---
api_key_in:
- query
api_specs:
- filename: cenevo-labguru-v1-openapi.yml
  format: yaml
  label: Labguru API v1
  slug: labguru-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cenevo/refs/heads/main/openapi/cenevo-labguru-v1-openapi.yml
- filename: cenevo-labguru-v2-openapi.yml
  format: yaml
  label: Labguru API v2
  slug: labguru-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cenevo/refs/heads/main/openapi/cenevo-labguru-v2-openapi.yml
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Cenevo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cenevo secures its APIs with token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cenevo
provider_slug: cenevo
scheme_count: 1
schemes:
- description: A session token created from a Labguru user login + password (and an optional account/workspace id) via POST /api/v1/sessions. The returned token is passed as the required `token` query parameter on every subsequent request. Organizations using SSO generate a personal token from the Labguru account settings page instead of using a password.
  in: query
  name: SessionToken
  parameter: token
  sources:
  - openapi/cenevo-labguru-v1-openapi.yml
  - openapi/cenevo-labguru-v2-openapi.yml
  sso: SSO customers generate a token from the account settings page rather than passing a password to the sessions endpoint.
  token_endpoint: https://my.labguru.com/api/v1/sessions
  token_request:
    body:
      account_id: (optional) account/workspace id to scope the token
      login: user e-mail
      password: user password
    method: POST
  type: token
slug: cenevo-authentication
source_filename: cenevo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.labguru.com/en/articles/6149483-api-introduction-and-overview\ndocs: https://help.labguru.com/en/articles/6149483-api-introduction-and-overview\nsummary:\n  types: [token]\n  api_key_in: [query]\n  oauth2_flows: []\n  note: >-\n    The Labguru API does not declare formal OpenAPI securitySchemes; it uses a\n    session-token model. Auth is not expressible as an OpenAPI securityScheme in\n    the published spec, so this profile is captured from the provider auth docs.\nschemes:\n- name: SessionToken\n  type: token\n  in: query\n  parameter: token\n  description: >-\n    A session token created from a Labguru user login + password (and an\n    optional account/workspace id) via POST /api/v1/sessions. The returned\n    token is passed as the required `token` query parameter on every subsequent\n    request. Organizations using SSO generate a personal token from the Labguru\n    account settings page instead of using\
  \ a password.\n  token_endpoint: https://my.labguru.com/api/v1/sessions\n  token_request:\n    method: POST\n    body:\n      login: user e-mail\n      password: user password\n      account_id: (optional) account/workspace id to scope the token\n  sso: >-\n    SSO customers generate a token from the account settings page rather than\n    passing a password to the sessions endpoint.\n  sources:\n  - openapi/cenevo-labguru-v1-openapi.yml\n  - openapi/cenevo-labguru-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cenevo/refs/heads/main/authentication/cenevo-authentication.yml
summary_line: token · 1 scheme
tags:
- Company
- Lab Automation
- Laboratory Informatics
- Electronic Lab Notebook
- LIMS
- Sample Management
- Life Sciences
- Biotechnology
- Scientific Research
- AI Agents
- Data Management
---
