---
anonymous_access: false
api_key_in: []
api_specs:
- filename: redreplier-com-alerts-api-openapi.yml
  format: yaml
  label: RedReplier Alerts API
  slug: redreplier-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-alerts-api-openapi.yml
- filename: redreplier-com-keywords-api-openapi.yml
  format: yaml
  label: RedReplier Keywords API
  slug: redreplier-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-keywords-api-openapi.yml
- filename: redreplier-com-mentions-api-openapi.yml
  format: yaml
  label: RedReplier Mentions API
  slug: redreplier-com-mentions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-mentions-api-openapi.yml
- filename: redreplier-com-websites-api-openapi.yml
  format: yaml
  label: RedReplier Websites API
  slug: redreplier-com-websites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-websites-api-openapi.yml
- filename: redreplier-com-workspaces-api-openapi.yml
  format: yaml
  label: RedReplier Workspaces API
  slug: redreplier-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-workspaces-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: RedReplier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RedReplier secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RedReplier
provider_slug: redreplier-com
scheme_count: 2
schemes:
- description: 'A RedReplier API token, sent as `Authorization: Bearer <api-key>`. Create one under API Tokens in the dashboard. An OAuth access token reaches every workspace its member belongs to: list them with `GET /workspaces` and pick one per call with the `X-Workspace-Id` header. An OAuth access token whose login has no RedReplier account answers 401 with `code: oauth_account_not_found`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/redreplier-com-openapi.json
  type: http
- description: 'Authorization code flow with PKCE or a client secret. Send the access token as `Authorization: Bearer <token>`. It reaches every workspace its member belongs to: list them with `GET /workspaces` and pick one per call with the `X-Workspace-Id` header. Ask for `offline_access` to receive a refresh token'
  flows:
  - authorizationUrl: https://cultured-oxygen-23.authkit.app/oauth2/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://cultured-oxygen-23.authkit.app/oauth2/token
  name: oauth2
  sources:
  - openapi/redreplier-com-openapi.json
  type: oauth2
slug: redreplier-com-authentication
source_filename: redreplier-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-23'\nmethod: derived\nsource: openapi/redreplier-com-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A RedReplier API token, sent as `Authorization: Bearer <api-key>`. Create one\n    under API Tokens in the dashboard. An OAuth access token reaches every workspace its member\n    belongs to: list them with `GET /workspaces` and pick one per call with the `X-Workspace-Id`\n    header. An OAuth access token whose login has no RedReplier account answers 401 with `code:\n    oauth_account_not_found`.'\n  sources:\n  - openapi/redreplier-com-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cultured-oxygen-23.authkit.app/oauth2/authorize\n    tokenUrl: https://cultured-oxygen-23.authkit.app/oauth2/token\n    scopes: 4\n  description: 'Authorization code flow with PKCE or\
  \ a client secret. Send the access token\n    as `Authorization: Bearer <token>`. It reaches every workspace its member belongs to: list\n    them with `GET /workspaces` and pick one per call with the `X-Workspace-Id` header. Ask\n    for `offline_access` to receive a refresh token'\n  sources:\n  - openapi/redreplier-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/redreplier-com/authentication/redreplier-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Reddit
- Lead-Generation
- AI
- Marketing
- Sales
---
