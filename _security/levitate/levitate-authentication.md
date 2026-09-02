---
api_key_in: []
api_specs:
- filename: levitate-companies-api-openapi.yml
  format: yaml
  label: Levitate Companies API
  slug: levitate-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-companies-api-openapi.yml
- filename: levitate-contacts-api-openapi.yml
  format: yaml
  label: Levitate Contacts API
  slug: levitate-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-contacts-api-openapi.yml
- filename: levitate-notes-api-openapi.yml
  format: yaml
  label: Levitate Notes API
  slug: levitate-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-notes-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Levitate Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Levitate secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Levitate
provider_slug: levitate
scheme_count: 1
schemes:
- description: Levitate OAuth2 Authorization Flow
  flows:
  - authorizationUrl: https://login.levitate.ai/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.levitate.ai/oauth2/token
  name: OAuth2
  sources:
  - openapi/levitate-public-v1-openapi.json
  type: oauth2
slug: levitate-authentication
source_filename: levitate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: openapi/levitate-public-v1-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.levitate.ai/oauth2/authorize\n    tokenUrl: https://login.levitate.ai/oauth2/token\n    scopes: 2\n  description: Levitate OAuth2 Authorization Flow\n  sources:\n  - openapi/levitate-public-v1-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/authentication/levitate-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- relationship-marketing
- CRM
- Email Marketing
- Contacts
- Small Business
- Insurance
- Financial-Services
- Non-Profit
- Marketing Automation
- MCP
- agent-native
- Software-as-a-Service
---
