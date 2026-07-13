---
api_key_in:
- query
api_specs:
- filename: zapier-partner-api.yml
  format: yaml
  label: Zapier Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-partner-api.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zapier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Zapier secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Zapier
provider_slug: zapier
scheme_count: 2
schemes:
- description: See our authentication documentation for how to find your Client ID
  in: query
  name: ClientIDAuthentication
  parameter: client_id
  sources:
  - openapi/zapier-partner-api.yml
  type: apiKey
- description: 'See our OAuth2 authentication documentation here: https://docs.zapier.com/powered-by-zapier/api-reference/authentication'
  flows:
  - authorizationUrl: https://zapier.com/oauth/authorize/
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://zapier.com/oauth/token/
  - authorizationUrl: https://zapier.com/oauth/authorize/
    flow: implicit
    scopes: 8
  name: OAuth
  sources:
  - openapi/zapier-partner-api.yml
  type: oauth2
slug: zapier-authentication
source_filename: zapier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zapier-partner-api.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: ClientIDAuthentication\n  type: apiKey\n  in: query\n  parameter: client_id\n  description: See our authentication documentation for how to find your Client ID\n  sources:\n  - openapi/zapier-partner-api.yml\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://zapier.com/oauth/authorize/\n    tokenUrl: https://zapier.com/oauth/token/\n    scopes: 8\n  - flow: implicit\n    authorizationUrl: https://zapier.com/oauth/authorize/\n    scopes: 8\n  description: 'See our OAuth2 authentication documentation here: https://docs.zapier.com/powered-by-zapier/api-reference/authentication'\n  sources:\n  - openapi/zapier-partner-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/authentication/zapier-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Integrations
- iPaaS
---
