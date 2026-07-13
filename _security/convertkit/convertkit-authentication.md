---
api_key_in:
- header
api_specs:
- filename: v4.json
  format: json
  label: Kit API
  slug: kit-api
  spec_type: OpenAPI
  url: https://developers.kit.com/api-reference/v4.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Convertkit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kit secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kit
provider_slug: convertkit
scheme_count: 2
schemes:
- description: Authenticate API requests via an API Key
  in: header
  name: API Key
  parameter: X-Kit-Api-Key
  sources:
  - openapi/openapi.json
  type: apiKey
- description: Authenticate API requests via an OAuth token
  flows:
  - authorizationUrl: https://api.kit.com/v4/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.kit.com/v4/oauth/token
  name: OAuth2
  sources:
  - openapi/openapi.json
  type: oauth2
slug: convertkit-authentication
source_filename: convertkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: X-Kit-Api-Key\n  description: Authenticate API requests via an API Key\n  sources:\n  - openapi/openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kit.com/v4/oauth/authorize\n    tokenUrl: https://api.kit.com/v4/oauth/token\n    scopes: 2\n  description: Authenticate API requests via an OAuth token\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/authentication/convertkit-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Email Marketing
- Creator Economy
- Subscribers
- Automation
- Newsletters
- Sequences
- Forms
- Broadcasts
---
