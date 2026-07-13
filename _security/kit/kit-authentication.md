---
api_key_in:
- header
api_specs:
- filename: kit-openapi.yml
  format: yaml
  label: Kit API V4
  slug: kit-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kit/refs/heads/main/openapi/kit-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Kit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kit secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kit
provider_slug: kit
scheme_count: 2
schemes:
- description: Personal API key issued from the Kit developer portal
  in: header
  name: ApiKeyAuth
  parameter: X-Kit-Api-Key
  sources:
  - openapi/kit-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://app.kit.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.kit.com/oauth/token
  name: OAuth2
  sources:
  - openapi/kit-openapi.yml
  type: oauth2
slug: kit-authentication
source_filename: kit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Kit-Api-Key\n  description: Personal API key issued from the Kit developer portal\n  sources:\n  - openapi/kit-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.kit.com/oauth/authorize\n    tokenUrl: https://api.kit.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/kit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kit/refs/heads/main/authentication/kit-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Email Marketing
- Creator Economy
- Newsletters
- Automation
- Subscribers
---
