---
anonymous_access: false
api_key_in: []
api_specs:
- filename: myagi-bot-contact-api-openapi.yml
  format: yaml
  label: Myagi Contact API
  slug: myagi-bot-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-contact-api-openapi.yml
- filename: myagi-bot-mcp-api-openapi.yml
  format: yaml
  label: Myagi MCP API
  slug: myagi-bot-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-mcp-api-openapi.yml
- filename: myagi-bot-well-known-api-openapi.yml
  format: yaml
  label: Myagi .well Known API
  slug: myagi-bot-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-well-known-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Myagi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Myagi secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Myagi
provider_slug: myagi-bot
scheme_count: 2
schemes:
- description: Public endpoints require no authentication.
  name: none
  scheme: noauth
  sources:
  - openapi/myagi-bot-openapi.json
  type: http
- description: OAuth 2.0 (discovery only as of 0.1.0).
  flows:
  - authorizationUrl: https://myagi.bot/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://myagi.bot/oauth/token
  name: oauth2
  sources:
  - openapi/myagi-bot-openapi.json
  type: oauth2
slug: myagi-bot-authentication
source_filename: myagi-bot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myagi-bot-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: none\n  type: http\n  scheme: noauth\n  description: Public endpoints require no authentication.\n  sources:\n  - openapi/myagi-bot-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://myagi.bot/oauth/authorize\n    tokenUrl: https://myagi.bot/oauth/token\n    scopes: 3\n  description: OAuth 2.0 (discovery only as of 0.1.0).\n  sources:\n  - openapi/myagi-bot-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/myagi-bot/authentication/myagi-bot-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AI Governance
- Cloud
- Governance
- Privacy
- Security
- Company
---
