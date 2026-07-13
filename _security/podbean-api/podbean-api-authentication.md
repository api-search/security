---
api_key_in:
- query
api_specs:
- filename: podbean-api-openapi.yml
  format: yaml
  label: Podbean API
  slug: podbean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean-api/refs/heads/main/openapi/podbean-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Podbean Api Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Podbean API secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Podbean API
provider_slug: podbean-api
scheme_count: 3
schemes:
- description: HTTP Basic for OAuth token requests (client_id / client_secret).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/podbean-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.podbean.com/v1/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/podbean-api-openapi.yml
  type: oauth2
- description: 'Podbean accepts the OAuth bearer token as the `access_token`

    query parameter on resource endpoints.'
  in: query
  name: accessTokenQuery
  parameter: access_token
  sources:
  - openapi/podbean-api-openapi.yml
  type: apiKey
slug: podbean-api-authentication
source_filename: podbean-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/podbean-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic for OAuth token requests (client_id / client_secret).\n  sources:\n  - openapi/podbean-api-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.podbean.com/v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/podbean-api-openapi.yml\n- name: accessTokenQuery\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: |-\n    Podbean accepts the OAuth bearer token as the `access_token`\n    query parameter on resource endpoints.\n  sources:\n  - openapi/podbean-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podbean-api/refs/heads/main/authentication/podbean-api-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Podcasts
- Podcasting
- Audio
- Media
- OAuth
- Episodes
---
