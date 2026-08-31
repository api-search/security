---
api_key_in:
- header
api_specs:
- filename: appfire-api-query-methods-api-openapi.yml
  format: yaml
  label: Appfire API query methods API
  slug: appfire-api-query-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/openapi/appfire-api-query-methods-api-openapi.yml
- filename: appfire-api-update-methods-api-openapi.yml
  format: yaml
  label: Appfire API update methods API
  slug: appfire-api-update-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/openapi/appfire-api-update-methods-api-openapi.yml
- filename: appfire-settings-api-openapi.yml
  format: yaml
  label: Appfire Settings API
  slug: appfire-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/openapi/appfire-settings-api-openapi.yml
- filename: appfire-worklogs-api-openapi.yml
  format: yaml
  label: Appfire Worklogs API
  slug: appfire-worklogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/openapi/appfire-worklogs-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Appfire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appfire secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Appfire
provider_slug: appfire
scheme_count: 3
schemes:
- bearerFormat: JWT
  docs: https://appfire.atlassian.net/wiki/spaces/7TFJ/pages/1253539983
  name: bearer
  product: 7pace Timetracker for Jira
  scheme: bearer
  sources:
  - openapi/appfire-7pace-timetracker-v1-openapi-original.yml
  - openapi/appfire-7pace-timetracker-v2-openapi-original.yml
  token_creation: Timetracker → Settings → API Tokens → + Create token (name + mandatory expiration date)
  type: http
- admin_surface: Users with the API_ADMIN_TABLE_ACCESS permission see an API administrator table and can list, rename and revoke any token in the organization.
  description: API authentication token generated from OKR module settings. Send only this header name (`API-Token`), not `Authorization` or `Authentication`.
  docs: https://developer.bigpicture.one/reference/okr-authentication
  in: header
  invalid_token_status: 401
  missing_header_status: 400
  name: API-Token
  parameter: API-Token
  product: Appfire OKR for Jira
  sources:
  - openapi/appfire-okr-openapi-original.json
  token_creation: Jira → Apps → OKR for Jira → Settings → API → Generate new token
  token_retrievable_later: false
  type: apiKey
- description: 'Authorization: Bearer <api token>, issued from the BigPicture UI. No scopes or granular permissions are documented.'
  docs: https://developer.bigpicture.one/reference/apitokens
  name: bearer
  product: BigPicture Cloud Public API
  scheme: bearer
  sources:
  - docs
  spec_available: false
  token_creation: BigPicture → API tokens (create, view, copy, revoke)
  type: http
slug: appfire-authentication
source_filename: appfire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: openapi/appfire-7pace-timetracker-v1-openapi-original.yml, openapi/appfire-7pace-timetracker-v2-openapi-original.yml,\n  openapi/appfire-okr-openapi-original.json\ndocs:\n- https://developer.bigpicture.one/reference/okr-authentication\n- https://developer.bigpicture.one/reference/apitokens\n- https://appfire.atlassian.net/wiki/spaces/7TFJ/pages/1253539983\nwarning: >-\n  Appfire's three public APIs use three different token conventions and two mutually exclusive header\n  names. Appfire OKR requires `API-Token` and explicitly forbids `Authorization`; 7pace Timetracker and\n  BigPicture both require `Authorization: Bearer`. A client written against one will not work against\n  another. No OAuth, no OIDC, and no scopes exist anywhere in the Appfire public API surface — every\n  token carries the full permissions of the user who minted it.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n\
  \  scopes: none\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  product: 7pace Timetracker for Jira\n  token_creation: Timetracker → Settings → API Tokens → + Create token (name + mandatory expiration date)\n  docs: https://appfire.atlassian.net/wiki/spaces/7TFJ/pages/1253539983\n  sources:\n  - openapi/appfire-7pace-timetracker-v1-openapi-original.yml\n  - openapi/appfire-7pace-timetracker-v2-openapi-original.yml\n- name: API-Token\n  type: apiKey\n  in: header\n  parameter: API-Token\n  product: Appfire OKR for Jira\n  description: >-\n    API authentication token generated from OKR module settings. Send only this header name\n    (`API-Token`), not `Authorization` or `Authentication`.\n  token_creation: Jira → Apps → OKR for Jira → Settings → API → Generate new token\n  token_retrievable_later: false\n  admin_surface: >-\n    Users with the API_ADMIN_TABLE_ACCESS permission see an API administrator table and can list,\n    rename and revoke any token\
  \ in the organization.\n  missing_header_status: 400\n  invalid_token_status: 401\n  docs: https://developer.bigpicture.one/reference/okr-authentication\n  sources:\n  - openapi/appfire-okr-openapi-original.json\n- name: bearer\n  type: http\n  scheme: bearer\n  product: BigPicture Cloud Public API\n  description: 'Authorization: Bearer <api token>, issued from the BigPicture UI. No scopes or granular permissions are documented.'\n  token_creation: BigPicture → API tokens (create, view, copy, revoke)\n  docs: https://developer.bigpicture.one/reference/apitokens\n  sources:\n  - docs\n  spec_available: false\ngaps:\n- No OAuth 2.0 or OpenID Connect on any Appfire API — no delegated authorization, no consent, no third-party app model.\n- No scopes on any token; least-privilege is not expressible.\n- Token rotation is documented only for 7pace (mandatory expiry). OKR and BigPicture tokens have no stated lifetime.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration\
  \ on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/authentication/appfire-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- atlassian
- jira
- confluence
- project-portfolio-management
- work-management
- time-tracking
- okr
- workflow-automation
- azure-devops
- marketplace-apps
- document-workflow
- enterprise-software
---
